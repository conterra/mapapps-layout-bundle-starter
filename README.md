# Layout-Bundle Starter
This bundle helps you to get started on providing layout descriptions for other bundles.

Installation Guide
------------------
1.  Download the bundle from release section
2.  Edit the layout descriptions inside the manifest.json
3.  Feel free to change whatever you want inside the bundle
3.  Upload the adjusted bundle to your map.apps installation or use it inside your development project

### Further Infos
http://developernetwork.conterra.de/en/documentation/mapapps/cookbook/customizing-windows-and-repositioned-widgtes-without-touching

Development Guide
------------------
### Define the mapapps remote base
Before you can run the project you have to define the mapapps.remote.base property in the pom.xml-file:
`<mapapps.remote.base>http://%YOURSERVER%/ct-mapapps-webapp-%VERSION%</mapapps.remote.base>`

##### Other methods to to define the mapapps.remote.base property.
1. Goal parameters
`mvn install -Dmapapps.remote.base=http://%YOURSERVER%/ct-mapapps-webapp-%VERSION%`

2. Build properties
Change the mapapps.remote.base in the build.properties file and run:
`mvn install -Denv=dev -Dlocal.configfile=%ABSOLUTEPATHTOPROJECTROOT%/build.properties`

