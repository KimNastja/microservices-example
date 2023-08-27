FROM openjdk:8-alpine
WORKDIR /usr/src/app

COPY . .
RUN chmod 777 mvnw \
    ./mvnw dependency:resolve \
    ./mvnw install

CMD ["java", "-jar", "./target/users-api-0.0.1-SNAPSHOT.jar"]
