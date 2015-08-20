# primrose-hibernate-simple
Simple Web Application using non-JPA Hibernate 5 and JTA on WildFly 10.

To run this on WildFly 10.0.0.Beta1, just do `mvn clean package` and copy `ear/target/primrose-hibernate-simple.ear` to `$WILDFLY_HOME/standalone/deployment directory`.

To run this on WildFly 9.0.1.Final you can do the same as for WildFly 10, however, following modificaitons must be done first:

* replace `hibernate5` with `hibernate4` in `./dao/src/main/resources/flowers-service.xml`
* replace `10.0.0.Beta1` with `9.0.1.Final` in `./pom.xml`
