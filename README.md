# Java, Spring Boot, Hello, Dockerfile
```
mvn package

java -jar target/demo-0.0.1-SNAPSHOT.jar

curl localhost:8080

Hello 1 12-23-2022 12:25:09 on unknown
```

```
docker build -t java-springboot-hello-docker .

docker run -i --rm -p 8080:8080 java-springboot-hello-docker

curl localhost:8080

Hello 1 12-23-2022 05:26:04 on fdfd462133ed
```