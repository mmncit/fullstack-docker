# fullstack-docker

Node, Express and Mongo backend

Container are static and volumes are dynamic and can be connected to container for handling db

Compose a docker image:

```console
$docker-compose build
```

Run the mongo service first:

Up a docker image to start with specific service

```console
$docker-compose up -d mongo
```

List the containers

```console
$docker ps
```

```console
$docker-compose up -d app
```

Stop the containers

```console
$docker-compose stop
```

Build the client docker image

```console
$cd client
$ docker build -t mmncit/client .
```

List the images

```console
$docker images
```

Run a container using this image

```console
$docker run -p 3000:3000 mmncit/client
```

Run the fullstack container

```console
$docker-compose build
$docker-compose up -d mongo # build the mongo, api and client in sequence
$docker-compose up -d api
$docker-compose up -d client
$docker ps # list the running containers
$docker-compose stop # stop the current container
```
