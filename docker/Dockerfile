####
# This Dockerfile is used in order to build a container that runs the Spring Boot application
# https://spring.io/guides/gs/spring-boot-docker/
# Build the image with:
# mvn package
# 
# docker build -t java-springboot-hello-docker .
#
# Then run the container using:
#
# docker run -i --rm -p 8080:8080 java-springboot-hello-docker
#
# curl localhost:8080
####
FROM openjdk:17
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]