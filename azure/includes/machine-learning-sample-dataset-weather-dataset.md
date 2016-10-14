Hourly land-based weather observations from NOAA (<a href="http://cdo.ncdc.noaa.gov/qclcd_ascii/, merged data from 201304 to 201310">merged data from 201304 to 201310</a>).<p> </p>The weather data covers observations made from airport weather stations, covering the time period April-October 2013. Before uploading to Azure ML Studio, the dataset was processed as follows:<ul><li>Weather station IDs were mapped to corresponding airport IDs</li><li>Weather stations not associated with the 70 busiest airports were filtered out</li><li>The Date column was split into separate Year, Month, and Day columns</li><li>The following columns were selected: AirportID, Year, Month, Day, Time, TimeZone, SkyCondition, Visibility, WeatherType, DryBulbFarenheit, DryBulbCelsius, WetBulbFarenheit, WetBulbCelsius, DewPointFarenheit, DewPointCelsius, RelativeHumidity, WindSpeed, WindDirection, ValueForWindCharacter, StationPressure, PressureTendency, PressureChange, SeaLevelPressure, RecordType, HourlyPrecip, Altimeter</li></ul>
