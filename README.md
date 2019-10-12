### Docker
 - Efficient
 - Lightweight
 - Self-Contained
 - Able to run safe anywhere and everywhere

**- Docker bundles your application into an image which is a standalone executable package.  Docker executes the image inside a container and the environment inside the container is completely isolated from the host machine.**

- https://hub.docker.com/_/node (Node versions and container setup)

- INFO on "bin/bash": https://unix.stackexchange.com/questions/398543/what-are-the-contents-of-bin-bash-and-what-do-i-do-if-i-accidentally-overwrote
- Dockerfile commands: https://docs.docker.com/engine/reference/builder/#usage

**Docker CLI Commands**

 - ``docker build -t superawesomecontainer .`` creates a Docker container
 - ``docker run -it superawesomecontainer`` runs the Docker container
 - ``docker run -it -p 3000:3000 superawesomecontainer`` runs Docker container using PORT
 - ``docker run -t -d superawesomecontainer`` runs Docker in the background
 - ``docker ps`` can see all the containers that are running
 - ``docker exec -it INSERT_HASH_HERE bash`` access to Docker container
 - ``docker stop INSERT_HASH_HERE`` stops container from running