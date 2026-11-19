FROM gradle:latest AS build
WORKDIR /src
COPY . .

FROM amazoncorretto:latest
WORKDIR /app
CMD ["java", "-jar", "catalog.jar"]
