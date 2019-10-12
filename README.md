### Docker:

**Docker bundles your application into an image which is a standalone executable package.  Docker executes the image inside a container and the environment inside the container is completely isolated from the host machine.**

 - Efficient
 - Lightweight
 - Self-Contained
 - Able to run safe anywhere and everywhere

Useful Links:

- https://hub.docker.com/_/node (Node container setup)
- INFO on "bin/bash": https://unix.stackexchange.com/questions/398543/what-are-the-contents-of-bin-bash-and-what-do-i-do-if-i-accidentally-overwrote
- Dockerfile commands: https://docs.docker.com/engine/reference/builder/#usage
- https://stackoverflow.com/questions/34809646/what-is-the-purpose-of-volume-in-dockerfile (Docker Volumes)
- https://www.linux.com/learn/docker-volumes-and-networks-compose (More on Docker Volumes)

**Docker Commands**

*(NOTE: everytime the yml files are changed you need to run: 'docker-compose build' to reread file)*
 - ``docker build -t superawesomecontainer .`` creates a Docker container
 - ``docker run -it superawesomecontainer`` runs the Docker container
 - ``docker run -it -p 3000:3000 superawesomecontainer`` runs Docker container using PORT
 - ``docker run -t -d superawesomecontainer`` runs Docker in the background
 - ``docker ps`` can see all the containers that are running
 - ``docker exec -it INSERT_HASH_HERE bash`` access to Docker container
 - ``docker stop INSERT_HASH_HERE`` stops container from running

 Docker Compose commands:
 - ``docker-compose build`` uses Docker Compose to build an image file
 - ``docker-compose run NAME_OF_API_OR_CONTAINER`` runs Docker Compose container
 - ``docker-compose down`` brings back down any Docker containers running in the background
 - ``docker-compose up --build`` command aggregates the output of each container  and builds initial container
 - ``docker-compose up`` to bring back up a Docker container prev. built
 - ``docker-compose up -d`` to bring back up container in the background
 - ``docker-compose exec NAME_OF_CONTAINER bash`` access to container bash