# docker network ls
# docker network inspect bridge
# docker run --name c1 -itd alpine ash
## communicate 
<!-- ## bridge default -->
# docker attach c1
 # ip addr show
 #  ping -c 5 172.17.0.3/16 container 2 (ip) only ip work in default network

 <!-- user bridge -->
# docker network create bridge --driver net1
# docker run --name c4 -itd --network net1 alpine ash