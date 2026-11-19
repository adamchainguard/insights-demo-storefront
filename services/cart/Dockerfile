FROM node:20 AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/nodejs22:latest
CMD ["server.js"]
