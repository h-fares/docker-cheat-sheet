# Docker Cheat Sheet
This Docker Cheat Sheet provides a quick reference to the most commonly used Docker commands. It covers essential tasks like setting up Docker containers, managing images, volumes, and networks, and orchestrating multi-container applications. Whether you're just getting started with Docker or looking to streamline your workflow, this cheat sheet will help you efficiently utilize Docker's powerful features.

## Docker Commands
### Setup and Configuration
`docker --version`: Check the Docker version installed on your system.

`docker info`: Display system-wide information about Docker.

### Working with Containers
`docker run [options] [image]`: Create and start a new container from an image.

`docker ps`: List all running containers.

`docker ps -a`: List all containers, including stopped ones.

`docker stop [container]`: Stop a running container.

`docker start [container]`: Start a stopped container.

`docker restart [container]`: Restart a running or stopped container.

`docker rm [container]`: Remove a stopped container.

`docker exec -it [container] [command]`: Execute a command inside a running container (e.g., docker exec -it my_container /bin/bash to open a bash shell).

### Managing Images
`docker images`: List all Docker images on your system.

`docker pull [image]`: Download an image from a Docker registry (e.g., Docker Hub).

`docker build -t [name] .`: Build an image from a Dockerfile in the current directory and tag it.

`docker rmi [image]`: Remove a Docker image.

`docker tag [image] [new-tag]`: Tag an image with a new name.

`docker push [image]`: Upload an image to a Docker registry.

### Networking
`docker network ls`: List all Docker networks.

`docker network create [name]`: Create a new Docker network.

`docker network inspect [name]`: Display detailed information about a network.

`docker network connect [network] [container]`: Connect a container to a network.

`docker network disconnect [network] [container]`: Disconnect a container from a network.

### Volumes
`docker volume ls`: List all Docker volumes.

`docker volume create [name]`: Create a new Docker volume.

`docker volume inspect [name]`: Display detailed information about a volume.

`docker volume rm [name]`: Remove a Docker volume.

### Docker Compose
`docker-compose up`: Create and start containers as defined in docker-compose.yml.

`docker-compose down`: Stop and remove containers, networks, and volumes created by docker-compose up.

`docker-compose ps`: List containers managed by Docker Compose.

`docker-compose build`: Build or rebuild services defined in docker-compose.yml.

`docker-compose logs`: View output from containers managed by Docker Compose.

### Useful Tips
`docker system prune`: Remove all unused containers, networks, images, and volumes.

`docker inspect [container/image]`: Return low-level information about a container or image.

`docker logs [container]`: Fetch the logs of a container.


