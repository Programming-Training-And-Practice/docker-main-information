




## Contents at a Glance.
* [About.](#about)
* [Documentation.](#documentation)
* [Help.](#help)





## About.





## Documentation.






| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| sudo systemctl status docker                                                |                                                                                 |
| sudo usermod -aG docker $USER                                               |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker -v                                                                   | Docker version.                                                                 | 





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




| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker images                                                               | List of locale docker images.                                                   |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker search [nameImage]                                                   | Search docker images in DockerHub.                                              |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker pull [nameImage]                                                     | Download docker image to local machine.                                         |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker ps                                                                   | Show which docker containers is running.                                        |
| docker ps -a                                                                | Show all docker containers that have been running at least once.                |
| docker ps -a -q                                                             |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker build -t [nameImage]:[nameTag] .                                     | Create docker image from local docker file.                                     |
| docker build -t quarkus/docker                                              |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker tag [imageName]:[imageTag] [imageName]:[imageTeg]                    |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker history quarkus/docker                                               |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker rm [containerID]                                                     | Remove docker container.                                                        |
| docker rm $(docker ps -qa)                                                  |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker rmi [imageID]                                                        | Remove docker image.                                                            |
| docker rmi [imageName]                                                      | Remove docker image.                                                            |
| docker rmi --force [imageID]                                                | Remove force docker image.                                                      |
| docker rmi --f [imageID]                                                    | Remove force docker image.                                                      |
| docker rmi $(docker images -q)                                              |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker exec -it [containerID] /bin/bash                                     | Enter to docker container to console.                                           |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker commit [containerID] [nameContainer]:[nameTag]                       |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker stop [containerID]                                                   | Stop docker container.                                                          |
| docker stop [nameContainer]                                                 | Stop docker container.                                                          |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker pause [containerID]                                                  | Pause docker container.                                                         |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker login                                                                |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker push [tag]                                                           |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker volume ls                                                            | Show docker volumes.                                                            |
| docker volume create [nameVolume]                                           | Create docker volumes.                                                          |





## Help.
