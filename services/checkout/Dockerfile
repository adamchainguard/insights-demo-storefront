FROM golang:latest AS build
WORKDIR /src
COPY go.mod main.go ./
RUN CGO_ENABLED=0 go build -o /out/checkout .

FROM debian:bookworm-slim
COPY --from=build /out/checkout /usr/local/bin/checkout
ENTRYPOINT ["checkout"]
