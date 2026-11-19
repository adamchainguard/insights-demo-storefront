FROM python:3.12 AS build
WORKDIR /src
COPY . .

FROM gcr.io/distroless/python3:latest
CMD ["app.py"]
