# Docker-Spring-Boot-App
Build a simple Spring Boot app with Docker

**Precondition**
* Install docker(1.6.0 or above)
* jdk(18 or above)
* Gradle(2.3 or above) or Maven(3.0 or above)
* clone this repo

**Run docker script**
* Use maven to build docker image
```sh
mvn package docker:build
```

OR 

* Use gradlew to docker image
```sh 
./gradlew build buildDocker
```

* Run the containerized application
```sh
docker images
docker run -p 8080:8080 -t gregturn/gs-spring-boot-docker
```
* Access the application on this link
```sh
http://localhost:8080
```