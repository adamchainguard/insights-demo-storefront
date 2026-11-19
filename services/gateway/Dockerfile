FROM golang:latest AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/static:latest
ENTRYPOINT ["/gateway"]
