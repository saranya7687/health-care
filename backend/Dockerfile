# Base image with java and Apline Linux
FROM eclipse-temurin:21-jdk-alpine

#Working Directory
WORKDIR /app

# Copy the Spring Boot jar file from local directory to the container
COPY target/auth-service-0.0.1-SNAPSHOT.jar app.jar

# Expose the application in the Spring Boot default port
EXPOSE 8080

# Inform docker to run Spring Boot using java
ENTRYPOINT ["java", "-jar", "app.jar"]
