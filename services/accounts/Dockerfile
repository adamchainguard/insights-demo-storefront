FROM maven:latest AS build
WORKDIR /src
COPY . .

FROM wildfly:latest
EXPOSE 8080
