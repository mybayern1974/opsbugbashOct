---
title: Continuous integration for Service Fabric | Microsoft Azure
description: Get an overview of how to set up continuous integration for a Service Fabric application by using Visual Studio Team Services (VSTS).
services: service-fabric
documentationcenter: na
author: mthalman-msft
manager: timlt
editor: ''

ms.service: multiple
ms.devlang: dotnet
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: multiple
ms.date: 08/01/2016
ms.author: mthalman

---
# Set up continuous integration for a Service Fabric application by using Visual Studio Team Services
This article describes the steps to set up continuous integration for an Azure Service Fabric application by using Visual Studio Team Services (VSTS), to ensure that your application is built, packaged, and deployed in an automated fashion.

This document reflects the current procedure and is expected to change over time.

## Prerequisites
To get started, follow these steps:

1. Ensure that you have access to a Team Services account or [create one](https://www.visualstudio.com/docs/setup-admin/team-services/sign-up-for-visual-studio-team-services) yourself.
2. Ensure that you have access to a Team Services team project or [create one](https://www.visualstudio.com/docs/setup-admin/create-team-project) yourself.
3. Ensure that you have a Service Fabric cluster to which you can deploy your application or create one using the [Azure Portal](service-fabric-cluster-creation-via-portal.md), an [Azure Resource Manager template](service-fabric-cluster-creation-via-arm.md), or [Visual Studio](service-fabric-cluster-creation-via-visual-studio.md).
4. Ensure that you have already created a Service Fabric Application (.sfproj) project. You must have a project that was created or upgraded with Service Fabric SDK 2.1 or higher (the .sfproj file should contain a ProjectVersion property value of 1.1 or higher).

> [!NOTE]
> Custom build agents are no longer required. Team Services hosted agents now come pre-installed with Service Fabric cluster management software, allowing for deployment of your applications directly from those agents.
> 
> 

## Configure and share your source files
The first thing you'll want to do is prepare a publish profile for use by the deployment process that will execute within Team Services.  The publish profile should be configured to target the cluster that you've previously prepared:

1. Choose a publish profile within your Application project that you want to use for your continuous integration workflow and follow the [publish instructions](service-fabric-publish-app-remote-cluster.md) on how to publish an application to a remote cluster. You don't actually need to publish your application though. You can simply click the **Save** hyperlink in the publish dialog once you've configured things appropriately.
2. If you want your application to be upgraded for each deployment that occurs within Team Services, you'll want to configure the publish profile to enable upgrade. In the same publish dialog used in step 1, ensure that the **Upgrade the Application** checkbox is checked.  Learn more about [configuring additional upgrade settings](service-fabric-visualstudio-configure-upgrade.md). Click the **Save** hyperlink to save the settings to the publish profile.
3. Ensure that you've saved your changes to the publish profile and cancel the publish dialog.
4. Now it's time to [share your Application project source files](https://www.visualstudio.com/docs/setup-admin/team-services/connect-to-visual-studio-team-services#vs) with Team Services. Once your source files are accessible in Team Services, you can now move on to the next step of generating builds. 

## Create a build definition
A Team Services build definition describes a workflow that is composed of a set of build steps that are executed sequentially. The goal of the build definition that you'll be creating is to produce a Service Fabric application package, as well as including some other supplemental files, that can be used to eventually deploy the application to a cluster. Learn more about Team Services [build definitions](https://www.visualstudio.com/docs/build/define/create).

### Create a definition from the build template
1. Open your team project in Visual Studio Team Services.
2. Select the **Build** tab.
3. Select the green **+** sign to create a new build definition.
4. In the dialog that opens, select **Azure Service Fabric Application** within the **Build** template category.
5. Select **Next**.
6. Select the repository and branch associated with your Service Fabric application.
7. Select the agent queue you wish to use. Hosted agents are supported.
8. Select **Create**.
9. Save the build definition and provide a name.
10. The following is a description of the build steps generated by the template:

| Build step | Description |
| --- | --- |
| Nuget restore |Restores the NuGet packages for the solution. |
| Build solution \*.sln |Builds the entire solution. |
| Build solution \*.sfproj |Generates the Service Fabric application package that will be used to deploy the application. Note that the application package location is specified to be within the build's artifact directory. |
| Update Service Fabric App Versions |Updates the version values contained in the application package's manifest files to allow for upgrade support. See the [task documentation page](https://go.microsoft.com/fwlink/?LinkId=820529) for more information. |
| Copy Files |Copies the publish profile and application parameters files to the build's artifacts in order to be consumed for deployment. |
| Publish Artifact |Publishes the build's artifacts. This allows a release definition to consume the build's artifacts. |

### Verify the default set of tasks
1. Verify the **Solution** input field for the **NuGet restore** and **Build solution** build steps.  By default, these build steps will execute upon all solution files that are contained in the associated repository.  If you only want the build definition to operate on one of those solution files, you need to explicitly update the path to that file.
2. Verify the **Solution** input field for the **Package application** build step.  By default, this build step assumes only one Service Fabric Application project (.sfproj) exists in the repository.  If you have multiple such files in your repository and want to target only one of them for this build definition, you need to explicitly update the path to that file.  If you want to package multiple Application projects in your repository, you need to create additional **Visual Studio Build** steps in the build definition that each target an Application project.  You would then also need to update the **MSBuild Arguments** field for each of those build steps so that the package location is unique for each of them.
3. Verify the versioning behavior defined in the **Update Service Fabric App Versions** build step.  By default, this build step appends the build number to all version values in the application package's manifest files. See the [task documentation page](https://go.microsoft.com/fwlink/?LinkId=820529) for more information. This is useful for supporting upgrade of your application since each upgrade deployment requires different version values from the previous deployment. If you're not intending to use application upgrade in your workflow, you may consider disabling this build step. In fact, it must be disabled if your intention is to produce a build that can be used to overwrite an existing Service Fabric application because deployment will fail if the version of the application produced by the build does not match the version of the application in the cluster.
4. If your solution contains a .NET Core project, you must ensure that your build definition contains a build step that restores the dependencies defined by any project.json files.  To do this, follow these steps:
   1. Select **Add build step...**.
   2. Locate the **Command Line** task within the Utility tab and click its Add button.
   3. For the task's input fields, use the following values:
   4. Tool: dotnet
   5. Arguments: restore
   6. Drag the task so that it is immediately after the **NuGet restore** step.
5. Save any changes you've made to the build definition.

### Try it
Select **Queue Build** to manually start a build. Builds will also be triggered upon push or check-in. Once you've verified that the build is executing successfully, you can now move on to defining a release definition that will deploy your application to a cluster.

## Create a release definition
A Team Services release definition describes a workflow that is composed of a set of tasks that are executed sequentially. The goal of the release definition that you'll be creating is to take an application package and deploy it to a cluster. When used together, the build definition and release definition can execute the entire workflow from starting with source files to ending with a running application in your cluster. Learn more about Team Services [release definitions](https://www.visualstudio.com/docs/release/author-release-definition/more-release-definition).

### Create a definition from the release template
1. Open your project in Visual Studio Team Services.
2. Select the **Release** tab.
3. Select the green **+** sign to create a new release definition and select **Create release definition** in the menu.
4. In the dialog that opens, select **Azure Service Fabric Deployment** within the **Deployment** template category.
5. Select **Next**.
6. Select the build definition you want to use as the source of this release definition.  The release definition will reference the artifacts that were produced by the selected build definition.
7. Check the **Continuous deployment** check box if you wish to have Team Services automatically create a new release and deploy the Service Fabric application whenever a build completes.
8. Select the agent queue you wish to use. Hosted agents are supported.
9. Select **Create**.
10. Edit the definition name by clicking the pencil icon at the top of the page.
11. Select the cluster to which your application should be deployed from the **Cluster Connection** input field of the task. The cluster connection provides the necessary information that allows the deployment task to connect to the cluster. If you do not yet have a cluster connection for your cluster, select the **Manage** hyperlink next to the field to add one. On the page that opens, perform the following steps:
    1. Select **New Service Endpoint** and then select **Azure Service Fabric** from the menu.
    2. Select the type of authentication being used by the cluster targeted by this endpoint.
    3. Define a name for your connection in the **Connection Name** field.  Typically, you would use the name of your cluster.
    4. Define the client connection endpoint URL in the **Cluster Endpoint** field.  Example: https://contoso.westus.cloudapp.azure.com:19000.
    5. For Azure Active Directory credentials, define the credentials you want to use to connect to the cluster in the **Username** and **Password** fields.
    6. For Certificate Based authentication, define the Base64 encoding of the client certificate file in the **Client Certificate** field.  See the help pop-up on that field for info on how to get that value.  If your certificate is password-protected, define the password in the **Password** field.
    7. Confirm your changes by clicking **OK**. After navigating back to your release definition, click the refresh icon on the **Cluster Connection** field to see the endpoint you just added.
12. Save the release definition.

The definition that is created consists of one task of type **Service Fabric Application Deployment**. See the [task documentation page](https://go.microsoft.com/fwlink/?LinkId=820528) for more information about this task.

### Verify the template defaults
1. Verify the **Publish Profile** input field for the **Deploy Service Fabric Application** task. By default, this field references a publish profile named Cloud.xml contained in the build's artifacts. If you want to reference a different publish profile or if the build contains multiple application packages in its artifacts, you need to update the path appropriately.
2. Verify the **Application Package** input field for the **Deploy Service Fabric Application** task. By default, this references the default application package path used in the build definition template.  If you've modified the default application package path in the build definition, you need to update the path appropriately here as well.

### Try it
Select **Create Release** from the **Release** button menu to manually create a release. In the dialog that opens, select the build that you want to base the release on and then click **Create**. If you enabled continuous deployment, releases will also be created automatically when the associated build definition completes a build.

## Next steps
To learn more about continuous integration with Service Fabric applications, read the following articles:

* [Team Services documentation home](https://www.visualstudio.com/docs/overview)
* [Build management in Team Services](https://www.visualstudio.com/docs/build/overview)
* [Release management in Team Services](https://www.visualstudio.com/docs/release/overview)

