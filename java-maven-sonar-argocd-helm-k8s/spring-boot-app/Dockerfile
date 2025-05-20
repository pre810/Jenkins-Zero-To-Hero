# Use a lightweight Java 17 JRE base image
FROM eclipse-temurin:17-jre

# Set the artifact path as a build argument
ARG artifact=target/spring-boot-web.jar

# Set working directory in the container
WORKDIR /opt/app

# Copy the Spring Boot JAR into the container
COPY ${artifact} app.jar

# Run the Spring Boot app
ENTRYPOINT ["java", "-jar", "app.jar"]
