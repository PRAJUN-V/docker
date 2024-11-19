# Learn Docker

- Tutorial followed: [CodeWithMosh](https://www.youtube.com/watch?v=pTFZFxd4hOI)
- Inside working dir create a file named: Dockerfile
- To check the docker hub created go to: https://hub.docker.com/

```sh
FROM python:3.12
COPY . /app
WORKDIR /app
CMD python main.py
```

```sh
docker build -t hello-docker .
```

To see all the docker images,
```sh
docker image ls
```

To run the docker image,
```sh
docker run <image-name>
```

To pull a docker image from docker hub,
```sh 
docker pull <image-name>
```

To see all the running containers,
```sh
docker ps
```

To see all containers (including stopped, exited, and running containers),
```sh
docker ps -a
```

To run ubuntu in interactive mode,
```sh
docker run -it ubuntu
```