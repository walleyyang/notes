#### Docker Compose

##### Run container
`docker-compose up`

##### Run container for specific compose file
`docker-compose -f specificfile.yml up`

##### Stop container
`docker-compose down`

##### Stop all containers
`docker stop $(docker ps -a -q)`

##### Remove all containers
`docker rm $(docker ps -a -q)`

##### Run container in background
`docker-compose up -d`

##### Build images before starting container
`docker-compose up --build`

##### Recreate container from existing image
`docker-compose up --force-recreate`

##### Prune containers
`docker container prune`

#### Containers

##### List all containers
`docker ps -a`

##### List running containers
`docker ps`

##### List stopped containers
`docker ps -f "status=exited"`

##### Remove container
`docker rm <container>`

##### Run named container
`docker start <container name>`

##### Stop named container
`docker stop <container name>`

##### Get into Bash in existing container
`docker exec -it <container name> bash`

#### Tag container to image (Commits the container changes to local image)
`docker commit <container> <image>`

#### Images

##### Build image and tag it
`docker build -t <image name>:<tag> .`

##### Remove image
`docker rmi <image>`

##### Prune dangling images (not tagged and not reference by any containers)
`docker image prune`

##### Prune all not be used by existing containers
`docker image prune -a`

##### Tag image
`docker tag <image> <repository>:<tag>`

##### Push tagged image to registry
`docker push <repository>:<tag>`

##### Run image from registry (tag is required if it's not the latest)
`docker container run <repository>:<tag>`

##### Run image interactive/pseudo tty (simulates terminal)
`docker container run -it <image>`

##### Run image with container name
`docker container run --name <name> <repository>:<tag>`

#### Volumes

##### List volume
`docker volume ls`

##### Remove volume
`docker volume rm <volume>`

##### Remove dangling volumes
`docker volume prune`

##### Remove all volume
`docker volume rm $(docker volume ls -q)`

#### Swarm

##### List stack in swarm
`docker stack ls`

##### Deploy stack to swarm
`docker stack deploy --compose-file docker-compose.yml <name>`

##### Remove stack from swarm
`docker stack rm <name>`

##### List containers from all nodes
`docker node ps $(docker node ls -q)`

##### List services in stack
`docker stack services <stack name>`

##### See log in a service
`docker service logs -f <service name>`

#### Miscellaneous
##### Clean everything
`docker system prune -a`

##### Save Image to tar
`docker save <image> > <image>.tar`

##### Load Image from tar
`docker load < <image>.tar`
