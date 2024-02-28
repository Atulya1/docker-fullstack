To build the image - 
docker image -t "name_of_the_image"

To see the images - 
docker images

To run a container - 
docker run -p port:port image_name

To list the containers - 
docker ps

To kill a container - 
docker kill docker_id

To stop a container - 
docker stop docker_id

To remove a container - 
docker rmi docker_id

To remove an image - 
docker rmi image_id


Docker compose allows managing multiple containers

To build a docker-compose - 
docker-compose up

If a certain container depends on another container, we need to run that container first
In our use-case, frontend depends on the backend, and backend depends on mongo
docker-compose up -d mongo
docker-compose up -d app
docker-compose up -d client
