# docker-mvn-j8-alpine
maven 3.3.9 on Alpine jdk8

Image on docker hub: [https://hub.docker.com/r/pengbai/docker-mvn-j8-alpine/](https://hub.docker.com/r/pengbai/docker-mvn-j8-alpine/)

This is a maven image, we can use maven command on running this image:

## Description

Pull image:
```
docker pull docker pull pengbai/docker-mvn-j8-alpine
```

Run ```mvn -version``` command with container, this container will on STATUS Exited after excuting this command, look container's logs (```docker logs CONTAINER_ID```) for more detail:
```
docker run -d  pengbai/docker-mvn-j8-alpine:3.3.9 mvn -version
```

The same to run other maven command, you can use volume to mount source on local.

