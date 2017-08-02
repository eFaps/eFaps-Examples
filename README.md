# eFaps-Examples
Example Repository

## First time installation

1.  check out repository
2.  verify settings for maven. A working example is used for the Travis automation [settings.xml](https://raw.githubusercontent.com/eFaps/Utils/master/settings/settings.xml)
3.  configure database
4.  mvn clean install
5.  mvn efaps:source-install


## Start webapp

mvn efaps-jetty:run
