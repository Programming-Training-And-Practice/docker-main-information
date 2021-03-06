# Docker Commands.




## Contents at a Glance.
* [About.](#about)
* [Documentation.](#documentation)
* [General Commands.](#general-commands)
* [Test Container.](#test-container)
* [docker build](#docker-build)
* [docker commit](#docker-commit)
* [docker exec](#docker-exec)
* [docker history](#docker-history)
* [docker images](#docker-images)
* [docker info](#docker-info)
* [docker login](#docker-login)
* [docker logs](#docker-logs)
* [docker pull](#docker-pull)
* [docker ps](#docker-ps)
* [docker pause](#docker-pause)
* [docker push](#docker-push)
* [docker run](#docker-run)
* [docker rm](#docker-rm)
* [docker rmi](#docker-rmi)
* [docker search](#docker-search)
* [docker stop](#docker-stop)
* [docker tag](#docker-tag)
* [docker v](#docker-v)
* [docker volume](#docker-volume)
* [docker network](#docker-network)
* [Help.](#help)





## About.





## Documentation.





## General Commands.

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| sudo systemctl status docker                                                |                                                                                 |
| sudo systemctl restart docker                                               |                                                                                 |
| sudo usermod -aG docker $USER                                               |                                                                                 |
| sudo du -sh /var/lib/docker                                                 |                                                                                 |
| docker system prune                                                         |                                                                                 |
| docker system prune -af --volumes                                           | Remove all unused containers, networks, images (both dangling and unreferenced), and volumes. |
| docker system prune -a --filter “until=2m”                                  |                                                                                 |
| docker system prune --filter “label=env=dev”                                | Remove the unused objects which have the label ‘env=dev’ by using the ‘–filter’ option |
| docker system prune --filter “label!=env=dev”                               | Remove all the objects that do not meet the mentioned condition                 |
|                                                                             |                                                                                 |

`docker run --rm -d --name postgres-prod -p 5432:5432 -e POSTGRES_PASSWORD=strong_password -e POSTGRES_USER=developer -e POSTGRES_DB=user-service-db-prod postgres`





## Test Container.
`docker run -ti --rm --memory=256m --cpus=2 openjdk:8u141-slim java -XX:+PrintFlagsFinal | grep MaxHeap`
`docker run -ti --rm --memory=256m --cpus=2 openjdk java -XX:+PrintFlagsFinal | grep MaxHeap`

`docker run -ti --rm --memory=256m --cpus=2 openjdk:8u141-slim java -XX:+PrintFlagsFinal | grep Thred`
`docker run -ti --rm --memory=256m --cpus=2 openjdk java -XX:+PrintFlagsFinal | grep Thred`




## docker v

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker -v                                                                   | Docker version.                                                                 | 
|                                                                             |                                                                                 |






## docker run

| Key/Command                                                                                                    | Description                                                                     |
| -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker run -it [nameImage]                                                                                     | Run docker in mod interactive.                                                  |   
| docker run -d [nameImage]                                                                                      | Run docker in mod demon.                                                        |
| docker run -p [localMachinePort]:[containerPort] [nameImage]                                                   | Run container and  configure ports.                                             |
| docker run --name [nameContainer] [nameImage]                                                                  | Run container and assign name to container.                                     |
| docker run --rm [nameImage]                                                                                    | After stop the container it will be remove.                                     |
| docker run -e [environmentValue]                                                                               | Assign environment variable.                                                    |
| docker run -v [absolutePathLocalMachineFolder]:[absolutePathContainerFolder]                                   | Run container and mount locale directory to container directory.                |
| docker run -v [nameVolume]:[absolutePathContainerFolder]                                                       | Run container and mount docker volume to container directory.                   |
| docker run -d -p 8282:8080 --name quarkusdocker quarkus/docker                                                 |                                                                                 |
| docker run --user=[nameUser] [nameImage]                                                                       | Run docker by not root user. Run docker by user "nameUser".                     |
| docker run --cap-add MAC_ADMIN [nameImage]                                                                     | Add capability MAC_ADMIN.                                                       |
| docker run --cap-drop MAC_ADMIN [nameImage]                                                                    | Remove capability MAC_ADMIN.                                                    |
| docker run --cap-add KILL [nameImage]                                                                          | Add capability KILL.                                                            |
| docker run --privileged [nameImage]                                                                            | Enable all capabilities.                                                        |
| docker run -d --name=[namePod] -p [localMachinePort]:[containerPort] --link [name]:[name] [nameImage]          |                                                                                 |
| docker run --label key=value [nameImage]                                                                       |                                                                                 |
|                                                                                                                |                                                                                 |





## docker images

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker images                                                               | List of locale docker images.                                                   |
| docker images ls                                                            | List of locale docker images.                                                   |
|                                                                             |                                                                                 |





## docker info

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker info                                                                 |                                                                                 |
| docker info | grep -i root                                                  |                                                                                 |
|                                                                             |                                                                                 |





## docker search

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker search [nameImage]                                                   | Search docker images in DockerHub.                                              |
|                                                                             |                                                                                 |






## docker pull

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker pull [nameImage]                                                     | Download docker image to local machine.                                         |
|                                                                             |                                                                                 |






## docker ps

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker ps                                                                   | Show which docker containers is running.                                        |
| docker ps -a                                                                | Show all docker containers that have been running at least once.                |
| docker ps -a -q                                                             |                                                                                 |
|                                                                             |                                                                                 |






## docker build

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker build -t [nameImage]:[nameTag] .                                     | Create docker image from local docker file.                                     |
| docker build -t quarkus/docker                                              |                                                                                 |
|                                                                             |                                                                                 |






## docker tag

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker tag [imageName]:[imageTag] [imageName]:[imageTeg]                    |                                                                                 |
|                                                                             |                                                                                 |






## docker history

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker history quarkus/docker                                               |                                                                                 |
|                                                                             |                                                                                 |






## docker rm

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker rm [containerID]                                                     | Remove docker container.                                                        |
| docker rm $(docker ps -qa)                                                  |                                                                                 |
| docker rm $(docker ps -a -f status=exited -q)                               |                                                                                 |
|                                                                             |                                                                                 |






## docker rmi

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker rmi [imageID]                                                        | Remove docker image.                                                            |
| docker rmi [imageName]                                                      | Remove docker image.                                                            |
| docker rmi --force [imageID]                                                | Remove force docker image.                                                      |
| docker rmi --f [imageID]                                                    | Remove force docker image.                                                      |
| docker rmi $(docker images -q)                                              |                                                                                 |
|                                                                             |                                                                                 |






## docker exec

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker exec -it [containerID] /bin/bash                                     | Enter to docker container to console.                                           |
| docker exec -ti [nameContainer] bash                                        |                                                                                 |
|                                                                             |                                                                                 |






## docker commit

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker commit [containerID] [nameContainer]:[nameTag]                       |                                                                                 |
|                                                                             |                                                                                 |






## docker stop

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker stop [containerID]                                                   | Stop docker container.                                                          |
| docker stop [nameContainer]                                                 | Stop docker container.                                                          |
| docker stop $(docker ps -qa)                                                |                                                                                 |
|                                                                             |                                                                                 |






## docker pause

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker pause [containerID]                                                  | Pause docker container.                                                         |
|                                                                             |                                                                                 |






## docker login

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker login                                                                |                                                                                 |
|                                                                             |                                                                                 |





## docker logs

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker logs -f [containerName]                                              |                                                                                 |
| docker logs -f ecf                                                          |                                                                                 |
|                                                                             |                                                                                 |





## docker push

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker push [tag]                                                           |                                                                                 |
|                                                                             |                                                                                 |






## docker volume

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker volume ls                                                            | Show docker volumes.                                                            |
| docker volume create [nameVolume]                                           | Create docker volumes.                                                          |
| docker system prune --volumes                                               | Delete all unused volumes                                                       |
|                                                                             |                                                                                 |





## docker network

| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker network create [nameNetwork]                                         |                                                                                 |
| docker network create --label key=value [nameNetwork]                       |                                                                                 |
| docker network connect [nameNetwork] [nameContainer]                        |                                                                                 |
| docker network inspect [nameNetwork]                                        |                                                                                 |
| docker network ls                                                           | Show docker networks                                                            |
| docker network prune                                                        | Remove all unused networks                                                      |
|                                                                             |                                                                                 |





## Help.
