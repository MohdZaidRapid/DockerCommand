a:docker pull imageName
# to pull an image from docker hub
#  docker pull hello-world:latest
b: docker images
# to find all images in our docker hub
# to search a specific  images
docker search imagename 
# for example docker search mysql

to search for containers list
# docker ps

# to run an container
# docker run imagename
docker run hello-world

# to info aboput all container ps
docker ps -a
docker inspect container name (for all info)


<!-- exmpale -->
# docker pull python-slim3.9
# docker run --name python-c1 python:3.9-slim

run container in background and return container id
# docker run --name python-c1 -d  python:3.9-slim 


 <!-- open in interactive mode it will remian in running state  -->
 # docker run --name python-c3 -i -t -d python:3.9-slim
 or
 # docker run --name python-c3 -it -d python:3.9-slim

<!-- execute a command in a running container -->
#  docker exec -it python-c3 python

<!-- remove container  after using it  -->
# docker run --name python-c5 --rm -it python:3.9-slim 
