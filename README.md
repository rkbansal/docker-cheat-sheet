# docker-cheat-sheet

## Hi Guys, here are some of most useful commands used in docker

##### `docker version` to get the version of docker
##### `docker run your_container_name_or_id_or_an_image` use this command to run a docker container
##### `docker run --name your_custom_name_for_container image_name` use this command to run a docker container with user defined name
##### `docker run -i your_container_name_or_id_or_an_image` use this command to run a docker container interactive mode (STDIN)

##### `docker run -it your_container_name_or_id_or_an_image` use this command to run a docker container interaction mode with terminal

##### `docker run -d your_container_name_or_id_or_an_image` use this command to run a docker container in detached mode (will run in background as a service)

##### `docker run your_container_name_or_id_or_an_image command` use this command to run a docker container with appended commands. eg. `docker run ubuntu sleep 100`

##### `docker exec your_container_name_or_id command` use this command to run a docker container with appended commands. eg. `docker exec my_container_name cat /etc/hosts`

##### `docker attach your_container_name_or_id` use this command to get attach with a detached container

##### `docker ps`

##### `docker ps -a`

##### `docker stop your_container_name_or_id`

##### `docker rm your_container_name_or_id`

##### `docker images`

##### `docker rmi your_image_name_or_id`

##### `docker inspect your_container_name_or_id`

##### `docker pull image_name`

##### `docker logs your_container_name_or_id`

##### `docker run -p your_port:docker_port your_container_name_or_id`

##### `docker run -v docker_host_dir:docker_container_directory your_container_name_or_id`

##### `docker run -e ENV_VARIABLE_NAME=VARIABLE_VALUE your_container_name_or_id`

##### `docker run --entrypoint your_entrypoint_command your_container_name_or_id your_command`
  eg. docker run --entrypoint sleep2.0 ubuntu-sleeper 10

### Networking commands
#### There are 3 types of networks in docker (Bridge, None, Host)
##### `docker run Ubuntu` (type -> Bridge) by default the container is available to every container inside the docker host
##### `docker run Ubuntu --network=none` (type -> None) doesn't connect the container to any other container
##### `docker run Ubuntu --network=host` (type -> Host) connect the server to the docker host on the same port, so it will be accessible outside of docker host

### Build from Dockerfile

##### `docker build ./` Current directory must have a Dockerfile

### Dockerfile commands

### `FROM` eg. FROM UBUNTU
### `ENTRYPOINT` eg. ENTRYPOINT["sleep"] won't get override by cmd arguments
### `CMD` eg. CMD sleep 100 or CMD["sleep", "100"] will get override by cmd arguments

