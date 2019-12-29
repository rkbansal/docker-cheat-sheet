# docker-cheat-sheet

## Hi Guys, here are some of most useful commands used in docker

##### `docker version` to get the version of docker
##### `docker run your_container_name_or_id_or_an_image` use this command to run a docker container

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
