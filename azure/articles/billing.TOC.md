# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-subscription-faq.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-buy-sign-up-azure-subscription.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-use-existing-office-365-account-azure-subscription.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-countries-and-currencies.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-buy-sign-up-azure-subscription#azure-offers---benefits-amp-limits.md)
# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-azure-subscription-past-due-balance.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-download-azure-invoice-daily-usage-date.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-set-up-alerts.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-understand-your-azure-marketplace-charges.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-understand-your-bill.md)
# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-how-to-cancel-azure-subscription.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](azure-subscription-service-limits.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-add-change-azure-subscription-administrator.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-subscription-become-disable.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-how-to-switch-azure-offer.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-subscription-transfer.md)
# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-how-to-change-azure-account-profile.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-add-office-365-tenant-to-azure-subscription.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-how-to-change-credit-card.md)
# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](https://msdn.microsoft.com/en-us/library/azure/1ea5b323-54bb-423d-916f-190de96c6a3c)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-usage-rate-card-overview.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-usage-rate-card-partner-solution-cloudcruiser.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-usage-rate-card-partner-solution-cloudyn.md)
# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-subscription-faq.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-credit-card-fails-during-azure-sign-up.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-cannot-login-subscription.md)
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-troubleshoot-azure-sign-up-issues.md)
# Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html
## [Usage : xmllint [options] XMLfiles ...
	Parse the XML files and output the result of the parsing
	--version : display the version of the XML library used
	--debug : dump a debug tree of the in-memory document
	--shell : run a navigating shell
	--debugent : debug the entities defined in the document
	--copy : used to test the internal copy implementation
	--recover : output what was parsable on broken XML documents
	--huge : remove any internal arbitrary parser limits
	--noent : substitute entity references by their value
	--noenc : ignore any encoding specified inside the document
	--noout : don't output the result tree
	--path 'paths': provide a set of paths for resources
	--load-trace : print trace of all external entities loaded
	--nonet : refuse to fetch DTDs or entities over network
	--nocompact : do not generate compact text nodes
	--htmlout : output results as HTML
	--nowrap : do not put HTML doc wrapper
	--valid : validate the document in addition to std well-formed check
	--postvalid : do a posteriori validation, i.e after parsing
	--dtdvalid URL : do a posteriori validation against a given DTD
	--dtdvalidfpi FPI : same but name the DTD with a Public Identifier
	--timing : print some timings
	--output file or -o file: save to a given file
	--repeat : repeat 100 times, for timing or profiling
	--insert : ad-hoc test for valid insertions
	--compress : turn on gzip compression of output
	--html : use the HTML parser
	--xmlout : force to use the XML serializer when using --html
	--nodefdtd : do not default HTML doctype
	--push : use the push mode of the parser
	--pushsmall : use the push mode of the parser using tiny increments
	--memory : parse from memory
	--maxmem nbbytes : limits memory allocation to nbbytes bytes
	--nowarning : do not emit warnings from parser/validator
	--noblanks : drop (ignorable?) blanks spaces
	--nocdata : replace cdata section with text nodes
	--format : reformat/reindent the input
	--encode encoding : output in the given encoding
	--dropdtd : remove the DOCTYPE of the input docs
	--pretty STYLE : pretty-print in a particular style
	                 0 Do not pretty print
	                 1 Format the XML content, as --format
	                 2 Add whitespace inside tags, preserving content
	--c14n : save in W3C canonical format v1.0 (with comments)
	--c14n11 : save in W3C canonical format v1.1 (with comments)
	--exc-c14n : save in W3C exclusive canonical format (with comments)
	--nsclean : remove redundant namespace declarations
	--testIO : test user I/O support
	--catalogs : use SGML catalogs from $SGML_CATALOG_FILES
	             otherwise XML Catalogs starting from 
	         file:///etc/xml/catalog are activated by default
	--nocatalogs: deactivate all catalogs
	--auto : generate a small doc on the fly
	--xinclude : do XInclude processing
	--noxincludenode : same but do not generate XInclude nodes
	--nofixup-base-uris : do not fixup xml:base uris
	--loaddtd : fetch external DTD
	--dtdattr : loaddtd + populate the tree with inherited attributes 
	--stream : use the streaming interface to process very large files
	--walker : create a reader and walk though the resulting doc
	--pattern pattern_value : test the pattern support
	--chkregister : verify the node registration code
	--relaxng schema : do RelaxNG validation against the schema
	--schema schema : do validation against the WXS schema
	--schematron schema : do validation against a schematron
	--sax1: use the old SAX1 interfaces for processing
	--sax: do not build a tree but work just at the SAX level
	--oldxml10: use XML-1.0 parsing rules before the 5th edition
	--xpath expr: evaluate the XPath expression, imply --noout

Libxml project home page: http://xmlsoft.org/
To report bugs or get some help check: http://xmlsoft.org/bugs.html](billing-how-to-create-billing-support-ticket.md)
