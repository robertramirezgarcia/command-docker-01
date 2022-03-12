# Course Docker Command
## Class 04

### Tag image: In this case we use CR of Azure
docker tag website:1.0.0 galaxydockerdev01.azurecr.io/website_robertramirezg:latest

### Here we will login

Url: galaxydockerdev01.azurecr.io
user: galaxydockerdev01

docker login *(Url)* -u *(user)*

docker login galaxydockerdev01.azurecr.io -u galaxydockerdev01

password: ac=gujhFScyEQANObYtribuR5NqYpHuI

### Here we will push
docker push galaxydockerdev01.azurecr.io/website_robertramirezg:latest

## Network

docker network ls
docker network create galaxy-net

docker run -d --net galaxy-net --name web01 -d nginx 
docker run -it --net galaxy-net  busybox sh

wget -q -O - http://web01:80/

docker inspect web01|grep galaxy-net

docker network connect galaxy-net a10efce35e13

docker network rm galaxy-net 

