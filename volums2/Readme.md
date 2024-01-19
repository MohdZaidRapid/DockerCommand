# docker volume create myvol
# docker volume inspect myvol
# docker volume ls
# docker run --name c1 -itd -v myvol:/myapp python
# docker run --name c2 -itd -v myvol:/myapp1 pyhon
# docker volume rm myvol
# docker run --name c2 -itd --volumes-from c1 
# docker run --name c1 -itd -v myvol python
# docker run --name c2 -itd --volumes-from c1 python
