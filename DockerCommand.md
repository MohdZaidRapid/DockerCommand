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

<!-- to stop container -->
docker start python-c3
docker stop python-c3
docker restart python-c3
****

<!-- remove container -->
docker rm container id

<!-- remove image -->
# docker rmi or with --force flag

<!-- This will remove all stopped containers -->
# docker container prune
# docker system prune

<!-- environment variable -->
# docker run --name mysql-c1 -e MYSQL_ROOT_PASSWORD=mohdzaid -d mysql 

<!-- mysql shell command -->
docker exec -it mysql-c1 mysql -u root -p

<!-- port map docker to our  machine -->
# docker run --name nginx-c1 -d -p 8080:80 nginx 

# FROM ubuntu


# WORKDIR /app


# COPY script.sh .


# RUN chmod +x script.sh

# CMD [ "./script.sh" ]

# docker build --no-cache -t mydockerimage .

# docker volume volume_name - It is used to create volume.

# docker volume Is -It is used to list volumes

# docker volume prune 
# docker volume inspect 
# docker volume rm volume name 
# docker volume prune rmeove all
# docker run -d --name container_name -v volume name:/app nginx -It is used to start a contaienr and create a volume if volume doesn's exists
(used with ro)


