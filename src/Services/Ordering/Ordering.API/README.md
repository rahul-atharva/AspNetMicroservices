# AspNetMicroservices Ordering.API
Ordering.API

# Docker Commands
 - docker pull mcr.microsoft.com/mssql/server  (https://hub.docker.com/_/microsoft-mssql-server)
 - mcr.microsoft.com/mssql/server:2017-latest
 - docker pull rabbitmq (https://hub.docker.com/_/rabbitmq)

## Close all dockers and run with below command on that location;

	docker-compose -f docker-compose.yml -f docker-compose.override.yml up --build
	or
	docker-compose -f docker-compose.yml -f docker-compose.override.yml up -d
	docker-compose -f docker-compose.yml -f docker-compose.override.yml down


# SQL Command
 -d :  detachment backgroudly

 
# Rabbit MQ
http://localhost:15672/ with guest and guest
  