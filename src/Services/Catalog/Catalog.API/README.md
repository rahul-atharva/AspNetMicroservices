# AspNetMicroservices Catalog.API
Catalog.API

# Docker Commands
 - docker pull mongo (https://hub.docker.com/_/mongo)
 - docker run -d -p 3000:3000 mongoclient/mongoclient  : Mongo Client (https://hub.docker.com/r/mongoclient/mongoclient)
 - docker ps
 - docker run -d -p 27017:27017 --name shopping-mongo mongo
 - docker exec -it shopping-mongo /bin/bash
 - docker logs -f shopping-mongo
 - cls

 - docker stop {3faa-imageid}
 - docker rm {3faa-imageid}
 - docker ps -s -- Show stopped images
 - docker images -- show images
 - docker ps -aq
 - docker stop $(docker ps -aq) - stop all docker image
 - docker rmi $(docker images -q) -- remove all images
 - docker system prune -- remove unnamed images

## Close all dockers and run with below command on that location;

	docker-compose -f docker-compose.yml -f docker-compose.override.yml up --build
	or
	docker-compose -f docker-compose.yml -f docker-compose.override.yml up -d
	docker-compose -f docker-compose.yml -f docker-compose.override.yml down


# Mongo Commands

1
-- Now we can open interactive terminal for mongo
docker exec -it shopping-mongo /bin/bash


2
-- After that, we are able to run mongo commands. 
Let me try with 

 - create database
 - create collection
 - add items into collection
 - list collection


ls
mongo
show dbs
use CatalogDb  --> for create db on mongo
db.createCollection('Products')  --> for create people collection

db.Products.insertMany([{ 'Name':'Asus Laptop','Category':'Computers', 'Summary':'Summary', 'Description':'Description', 'ImageFile':'ImageFile', 'Price':54.93 }, { 'Name':'HP Laptop','Category':'Computers', 'Summary':'Summary', 'Description':'Description', 'ImageFile':'ImageFile', 'Price':88.93 } ])

db.Products.insertMany(
			[
			    {
			        "Name": "Asus Laptop",
			        "Category": "Computers",
			        "Summary": "Summary",
			        "Description": "Description",
			        "ImageFile": "ImageFile",
			        "Price": 54.93
			    },
			    {
			        "Name": "HP Laptop",
			        "Category": "Computers",
			        "Summary": "Summary",
			        "Description": "Description",
			        "ImageFile": "ImageFile",
			        "Price": 88.93d
			    }
			])

db.Products.find({}).pretty()
db.Products.remove({})

show databases
show collections
db.Products.find({}).pretty()



