# Learn Docker

Inside working dir create a file named: Dockerfile
To check the docker hub created go to: https://hub.docker.com/

```sh
FROM python:3.12
COPY . /app
WORKDIR /app
CMD python main.py
```

```sh
docker build -t hello-docker .
```

