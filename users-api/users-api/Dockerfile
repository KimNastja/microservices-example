FROM openjdk:8-alpine

RUN chmod 777 mvnw \
    ./mvnw dependency:resolve \
    ./mvnw install
WORKDIR /usr/src/app
COPY . .


CMD ["java", "-jar", "./target/users-api-0.0.1-SNAPSHOT.jar"]
