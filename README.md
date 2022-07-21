# fullstack-docker

Node, Express and Mongo backend

Build a docker image:

```console
$docker build -t mmncit/simple-backend .
```

List the images:

```console
$docker images
```

Remove docker image

```console
$docker rmi <IMAGE ID>
```

Run docker image

```console
$docker run -p 4000:4000 mmncit/simple-backend
```

List the containers

```console
$docker ps
```

Stop container

```console
$docker stop <CONTAINER NAME>
```
