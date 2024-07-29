# Use OpenJDK 17 base image
FROM openjdk:17-alpine

# Expose the port your application will run on
EXPOSE 8070

# Set the application home directory
ENV APP_HOME /usr/src/app

# Copy the JAR file into the container
COPY target/shopping-cart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

# Set the working directory
WORKDIR $APP_HOME

# Set the entry point to run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
