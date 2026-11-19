FROM rust:latest AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/cc:latest
ENTRYPOINT ["/recommendations"]
