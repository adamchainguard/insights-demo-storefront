FROM cgr.dev/0-cve.com/python:latest-dev AS build
WORKDIR /srv
COPY search.py .

FROM cgr.dev/0-cve.com/python:latest
WORKDIR /srv
COPY --from=build /srv/search.py .
ENTRYPOINT ["python", "search.py"]
