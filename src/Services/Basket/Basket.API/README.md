# AspNetMicroservices Basket.API
Basket.API

# Docker Commands
 - docker pull redis

## Close all dockers and run with below command on that location;

	docker-compose -f docker-compose.yml -f docker-compose.override.yml up --build
	or
	docker-compose -f docker-compose.yml -f docker-compose.override.yml up -d
	docker-compose -f docker-compose.yml -f docker-compose.override.yml down


# Redis Command
 -d :  detachment backgroudly

 - docker run -d -p 6379:6379 --name aspnetrun-redis redis
 - docker logs -f aspnetrun-redis

 for troubleshooting OR Interactive Terminal
  - docker exec -it aspnetrun-redis /bin/bash
  - redis-cli
  - ping
  - set key value 
  - get key
  - set name rahul
  - get name
  