#Docker Main Information.





## Contents at a Glance.
* [About.](#about)
* [Documentation.](#documentation)
* [Help.](#help)





## About.





## Documentation.
* [Docker.](https://www.docker.com/)
* [Docker Engine.]()
* [Docker Container.]()
* [Docker Image.]()
* [Dockerfile.]()
* [DockerHub.]()
* []()





## Commands.
* `sudo systemctl status docker`
* `sudo usermod -aG docker $USER`<br/><br/>


* `docker -v` Docker version.<br/><br/>

* `docker run -it -p 8282:8080 nameImage` Run docker in mod interactive.
* `docker run -d -p 8282:8080 nameImage` Run docker in mod demon.
* `docker run -d -p 8282:8080 --name quarkusdocker quarkus/docker`<br/><br/>

* `docker images` List of locale docker images.<br/><br/>

* `docker search nameImage` Search docker images in DockerHub.<br/><br/>

* `docker pull nameImage` Download docker image to local machine.<br/><br/>

* `docker ps` Show which docker containers is running.
* `docker ps -a` Show all docker containers that have been running at least once.<br/><br/>

* `docker build -t nameImage:nameTag .`Create docker image from local docker file.
* `docker build -t quarkus/docker`<br/><br/>

* `docker tag imageName:imageTag imageName:imageTeg`

* `docker history quarkus/docker`<br/><br/>

* `docker rm containerID` Remove docker container.<br/><br/>

* `docker rmi imageID` Remove docker image.
* `docker rmi --force imageID` Remove force docker image.
* `docker rmi --f imageID` Remove force docker image.<br/><br/>

* `docker exec -it containerID /bin/bash` Enter to docker container to console.

* `docker commit containerID nameContainer:nameTag`

* `docker stop containerID` Stop docker container.

* `docker pause containerID` Pause docker container.





## Help.
