# thani-prime
This is an RESTful API, built in Java 8, using Spring Boot framework, which when invoked without any param, it will generate prime numbers upto 2^63-1. Long.MAX_VALUE
There are 2 path params for the API, Strategy, and Upper limit. Strategy could be defaulted and is optional. there are 2 options build to generate the Prime numbers
these options can be queried by one of the endpoints. The 2 prime number generation techniques built are iterative approach, and Fork join approach.
there is also option built to cache the results, so it can be queried using the result id (UUID) to retrieve the results without the need to generate it again
caching and fork join options have been done to aid with performance 
This project uses Maven as the build tool
API documentation is done using Swagger and can be accessed from the Swagger-UI

Pre-requisites - Java 8, Maven 3.8.2 & above
Build steps - mvn clean install 
running the micro service in integrated tomcat - java -jar target/thani-prime-0.0.1-SNAPSHOT.jar
