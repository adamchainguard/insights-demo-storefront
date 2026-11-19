FROM maven:latest AS build
WORKDIR /src
COPY pom.xml .
COPY src ./src
RUN mvn -q -DskipTests package

FROM eclipse-temurin:21-jre
COPY --from=build /src/target/inventory.jar /app/inventory.jar
ENTRYPOINT ["java", "-jar", "/app/inventory.jar"]
