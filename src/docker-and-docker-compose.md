# Docker and docker-compose

A set of the valuable docker and docker-compose commands.

## Docker commands

```bash
# ----- basic management -----

# list of active containers:
docker container ls

# list of active and disabled containers:
docker container ls -a

# list of volumes:
docker container volume ls

# list of networks:
docker container network ls

# ----- building -----

# build a docker container based on the Docker file in the directory:
docker build -t image-name:tag

# ----- running -----

# starting a container:
docker run --name container-name image-name:tag .

# additional port mapping:
docker run -p computer-port:container-port image-name:tag

# additional network assignment:
docker run --network network-name image-name:tag

# additional env variable:
docker run -e env-variable-name=admin image-name:tag

# additional volume assign and directory in the container mapping: (-v container_data:/app)
docker run -v volumen-name:/catalog-in-the-container image-name:tag

# passing the env values from the file:
docker run --env-file C:\Users\wmarek\Git\dk-tax\ELO-sap38-jobs-web\.env 

# detach terminal mode:
docker run -d image-name:tag

# ----- stopping -----

docker stop container-name

# ----- removing -----

# remove the container:
docker rm container-name

# remove the image:
docker rmi image-name

# ----- bash -----

# connects to the container's bash (if available):
docker exec -it container-name bash

# connects to the container's shell (if available):
docker exec -it container-name sh
```

## Docker-compose commands

```bash
docker-compose build
docker-compose up
docker-compose up -d
docker-compose stop
docker-compose rm
```