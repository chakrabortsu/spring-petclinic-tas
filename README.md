Spring Petclinic
================

## Running the application on Cloud Foundry

* Install cf cli tool.
* Clone repository `git clone https://github.com/chakrabortsu/spring-petclinic-tas.git`.
* The provided manifest uses an external database to create and bind database services to the application, so we need to create as a pre-requisite before pushing the application
~~~
# view the services available
$ cf marketplace
# create a service instance
$ cf create-service <service> <service plan> <service name>
$ cf create-service p.mysql small spring-petclinic-db

* Build and push the application.

$ cd spring-petclinic-tas
$ cf push



