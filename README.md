# Introduction To Docker

## Story

It's a couple of hours before your first job interview. In the job listing, they mentioned that a minimal mongodb experience is a nice to have. You are attempting to remember anything about mongo commands, but they just won't come. With your limited amount of time left before the interview, it would be nice if you could setup a very simple environment to practice mongo commands in, without needing to create a database and a server for it.

## What are you going to learn?

- How to handle the Docker CLI and effectively use containers.

## Tasks

1. Create a container that is running the MongoDB server, then join to it and run the Mongo cli inside.
    - A container that runs a MongoDB server.
    - Mongo cli is running.

## General requirements

None

## Hints

- Whenever you need to supply a randomly generated id in Docker (e.g. a container id), it's enough to type the first few characters of it. Even one character works if it's unique!
- When you would like to clear all of the things that Docker cached on your computer (this can free up disk space and prevent your Docker from using outdated resources, as it forces everything to repull/reinstall inside Docker), type
```
docker system prune -af
```
However, this will make your next Docker runs slower because of the redownloading

- If you get an error message like this when  trying to push docker image to ECR:
```
Error message: denied: User: …. Is not authorized to perform: …. ecr:InitiateLayerUpload on resource ….
```
It can be that you logged in with another account at aws cli.
To fix the problem, configure your local aws cli with **your** aws user credentials.

## Background materials

* <i class="far fa-exclamation"></i> [Mongo Docker Image](https://hub.docker.com/_/mongo)
* <i class="far fa-exclamation"></i> [Mongo CLI for Testing the containers](https://docs.mongodb.com/manual/mongo/)
* <i class="far fa-exclamation"></i> [AWS Named Profiles](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-profiles.html)
* <i class="far fa-video"></i> [Docker with Nana](https://youtu.be/3c-iBn73dDE)
* <i class="far fa-video"></i> [Docker basics](https://youtu.be/p28piYY_wv8)
