# maven-spring-boot
I initially started off with creating a Hello World Maven project by following:

`https://maven.apache.org/guides/getting-started/index.html`

I could also have followed the [Maven in 5 Minutes](https://maven.apache.org/guides/getting-started/maven-in-five-minutes.html) guide.

To compile, test and package the application first:

`cd rdp-app/`

then run:

`mvn clean package`

To then run the main method:

`java -jar target/rdp-app-1.0-SNAPSHOT.jar`

This will start Spring. Spring Boot's embedded Apache Tomcat server is acting as a webserver and listening for requests on `localhost:8080`. The code has made the `/hello` endpoint available, with an optional `name` parameter:

```
http://localhost:8080/name           # displays Hello World!
http://localhost:8080/hello?name=Amy # displays Hello Amy!
```
