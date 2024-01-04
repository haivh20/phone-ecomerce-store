Build dockerfile

FROM openjdk:17
WORKDIR /app
COPY target/my-spring-boot-app-0.0.1-SNAPSHOT.jar /app/my-app.jar
EXPOSE 8080
ENTRYPOINT ["java","-jar","/app/my-app.jar"]
