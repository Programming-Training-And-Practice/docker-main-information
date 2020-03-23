




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





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker run -it -p 8282:8080 nameImage                                       | Run docker in mod interactive.                                                  |   
| docker run -d -p 8282:8080 nameImage                                        | Run docker in mod demon.                                                        |
| docker run -d -p 8282:8080 --name quarkusdocker quarkus/docker              |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker images                                                               | List of locale docker images.                                                   |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker search nameImage                                                     | Search docker images in DockerHub.                                              |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker pull nameImage                                                       | Download docker image to local machine.                                         |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker ps                                                                   | Show which docker containers is running.                                        |
| docker ps -a                                                                | Show all docker containers that have been running at least once.                |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker build -t nameImage:nameTag .                                         | Create docker image from local docker file.                                     |
| docker build -t quarkus/docker                                              |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker tag imageName:imageTag imageName:imageTeg                            |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker history quarkus/docker                                               |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker rm containerID                                                       | Remove docker container.                                                        |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker rmi imageID                                                          | Remove docker image.                                                            |
| docker rmi --force imageID                                                  | Remove force docker image.                                                      |
| docker rmi --f imageID                                                      | Remove force docker image.                                                      |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker exec -it containerID /bin/bash                                       | Enter to docker container to console.                                           |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker commit containerID nameContainer:nameTag                             |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker stop containerID                                                     | Stop docker container.                                                          |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker pause containerID                                                    | Pause docker container.                                                         |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker login                                                                |                                                                                 |





| Key/Command                                                                 | Description                                                                     |
| --------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| docker push [tag]                                                           |                                                                                 |





## Help.
