FROM golang:1.24 AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/static-debian12:latest
ENTRYPOINT ["/shipping"]
