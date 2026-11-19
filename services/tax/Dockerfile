FROM golang:latest AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/base:latest
ENTRYPOINT ["/tax"]
