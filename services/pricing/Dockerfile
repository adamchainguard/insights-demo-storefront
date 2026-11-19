FROM maven:latest AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/java21:latest
CMD ["pricing.jar"]
