# eFaps-Examples
Example Repository

## First time installation

1.  Clone this repository
2.  Verify settings for maven. A working example is used for the Travis automation [settings.xml](https://raw.githubusercontent.com/eFaps/Utils/master/settings/settings.xml)
3.  Change directory to ElementalInstall 
3.  Configure a database as shown in [pom.xml](https://github.com/eFaps/eFaps-Examples/blob/master/ElementalInstall/pom.xml) or alter configuration of the efaps-maven-plugin. Especially the connection properties.
4.  run `mvn clean install`  
5.  run `mvn efaps:source-install`  -> this will create all data entries needed. (Normally it will be necessary to run it at least twice or threee times untill all elements are created successfullly. It is known to be a little bit "problematic" but solving the known issued is not high priority)


## Start webapp

1.  run `mvn efaps-jetty:run`  (Check plugin configuration for the database. Same configuration as for the efaps-maven-plugin should be used for the efaps-jetty-maven-plugin)
2.  Open http://localhost:8888/eFaps/ and login with Administrator Administrator
