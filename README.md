# primrose-hibernate-simple
Simple Web Application using non-JPA Hibernate 5 and JTA on WildFly 10.

To run this on WildFly 10.0.0.Final, just do `mvn clean package` and copy `ear/target/primrose-hibernate-simple.ear` to `$WILDFLY_HOME/standalone/deployment directory`.

To reproduce the *.tld file loading issue, comment out the spring-webmvc dependency in `war/pom.xml` and uncomment it in `ear/pom.xml` so that is will land in `EAR/lib` directory instead of `EAR/primrose-hibernate-simple-war/WEB-INF/lib` directory.
