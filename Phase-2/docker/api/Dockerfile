FROM openjdk:8-jdk

# Install build essentials for C
RUN apt-get update && \
    apt-get install -y build-essential

WORKDIR /usr/src/app

COPY . .

# Compile the C components
RUN cd c && \
    make

# Build the Java components
RUN cd java && \
    ./gradlew build

EXPOSE 8080

# Define the command to run the API
CMD ["java", "-jar", "path/to/java/application.jar"]
