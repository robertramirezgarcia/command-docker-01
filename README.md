# Course Docker Command
# Class 04

##Tag image
## In this case we use CR of Azure
docker tag website:1.0.0 galaxydockerdev01.azurecr.io/website_robertramirezg:latest

Url: galaxydockerdev01.azurecr.io
user: galaxydockerdev01

##Here we will login
docker login galaxydockerdev01.azurecr.io -u galaxydockerdev01

password: ac=gujhFScyEQANObYtribuR5NqYpHuI

##Here we will push
docker push galaxydockerdev01.azurecr.io/website_robertramirezg:latest
