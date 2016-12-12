# Spring_Docker_By_Gradle
These codes are for demonstrating two aspects of the assignment, In the first we will use the Gradle and Spring Boot. And in the second we will use the Gradle, Spring Boot in a docker image.
First Aspect
-------------
Here we are simply using the Gradle and a sample Spring Boot application. So please refer the build - Copy for local host run.gradle file as the build.gradle file.The docker file is same in both the aspect. The Application.Java which is a simple message demonstration is also same in both the aspect.
Please note that the command for wrapper is (keeping in mind we are in correct directory): gradle wrapper --gradle-version 2.13
Please note that the command for build and running the Java application (keeping in mind we are in correct directory): ./gradlew build && java -jar build/libs/gs-spring-boot-docker-0.1.0.jar

Second Aspect
-------------
Here we are using the Docker power to containerized the Spring boot application leveraging the Gradle. So please refer the build - Copy for docker run.gradle file as the build.gradle.file. The docker file is same in both the aspect. The Application.Java which is a simple message demonstration is also same in both the aspect.
Please note that the command for wrapper is (keeping in mind we are in correct directory): gradle wrapper --gradle-version 2.13
Please note that the command for build:./gradlew build buildDocker
Please note that the command for seeing the available images: $ docker images
please note that the command for runnign the image: $ docker run -p 8080:8080 -t mona2989lisa/gradlet
please note that the command for seeing the running images: $ docker ps
Please note that the command for stopping the image:$ docker stop c8c56a34ecae (the container id is the paramter)

Please refer the emailed word document "Docker_gradle_Spring" for the details and the screen shots.
