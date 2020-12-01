# Alpine Linux with OpenJDK JRE
## FROM tells which base image to use for creating image. Base impage is open jdk here
FROM openjdk:8-jre-alpine

# Copy war file. This is copy the war file to the image
COPY DockerAPI-0.0.1-SNAPSHOT.jar /DockerAPI.war

# run the app
CMD ["/usr/bin/java", "-jar", "/DockerAPI.war"]



