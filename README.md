# docker-mvn-j8-alpine
Maven on Alpine OpenJDK8

[![](https://badge.imagelayers.io/pengbai/docker-mvn-j8-alpine:latest.svg)](https://imagelayers.io/?images=pengbai/docker-mvn-j8-alpine:latest 'Get your own badge on imagelayers.io')

Image on docker hub: [https://hub.docker.com/r/pengbai/docker-mvn-j8-alpine/](https://hub.docker.com/r/pengbai/docker-mvn-j8-alpine/)

This is a maven image, we can use maven command on running this image:

## Description

Pull image:
```
docker pull docker pull pengbai/docker-mvn-j8-alpine
```

Run ```mvn -version``` command with container, this container will on STATUS Exited after excuting this command, look container's logs (```docker logs CONTAINER_ID```) for more detail:
```
docker run -d pengbai/docker-mvn-j8-alpine:3.3.9 mvn -version
```

The same to run other maven command THIS_IS_A_MVN_COMMAND, you can also use volume to mount source on local /local-workspace.
```
docker run -d -v /local-workspace:/container-workspace pengbai/docker-mvn-j8-alpine:3.3.9 THIS_IS_A_MVN_COMMAND
```

