# Use a base image with JDK
FROM openjdk:17-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the JAR file built by Maven/Gradle to the container
COPY target/com.example-0.0.1-SNAPSHOT.jar /app/com.example.jar

# Expose port 8080 on which the application will run
EXPOSE 8080

# Run the JAR file
ENTRYPOINT ["java", "-jar", "com.example.jar"]
