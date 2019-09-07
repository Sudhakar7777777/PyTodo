# Simple TODO APP

A basic todo app using Python, Flask, React, MongoDB and Docker.
To run this on local machine, follow these steps after cloning the repository.

PS: Assuming that docker & docker-compose are already configured on your machine.

## Install npm dependencies
```
 yarn install
```

## To start and load the front-end app from docker container.
```
yarn run build
docker-compose up --build
```
You will be able to access the app on http://localhost:4000

## To run UI in webpack-dev-server & backend in docker container.
```
docker-compose up --build
yarn run serve
```
You will be able to access the app on http://localhost:8080

## Helpful Commands

```
docker-compose up --build
```

## How to login to mongo db image and validate db values

```
> docker ps

> docker exec -it <container name> /bin/bash
eg:
> docker exec -it mongodb /bin/bash

Once you have access to bash shell, connect to the Mongo instance.Mongodb
> mongo
> show dbs
> use todoDev
> show collections
> db.users.find()
```

###### Reference:
https://medium.com/@riken.mehta/full-stack-tutorial-flask-react-docker-420da3543c91
