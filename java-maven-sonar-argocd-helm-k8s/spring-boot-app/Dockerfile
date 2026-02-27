# Use Java 11 runtime
FROM adoptopenjdk/openjdk11:alpine-jre

# Path to your JAR (can be overridden at build time)
ARG artifact=target/spring-boot-web.jar

# Set working directory
WORKDIR /opt/app

# Copy the built Spring Boot JAR
COPY ${artifact} app.jar

# Entry point for the container
ENTRYPOINT ["java","-jar","app.jar"]
