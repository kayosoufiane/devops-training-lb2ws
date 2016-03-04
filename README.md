# DevOps Training - Load balancing of 2 web servers - Practical - using Docker compose


## Usage

### Start all services

```
cd devops-lb2ws-training

docker-compose up -d
```

### Test web servers :
http://localhost:5011/
http://localhost:5012/
http://localhost:5050/

### Stop the web server A
```
docker kill mywebserver.a
```

### Test web servers :
http://localhost:5011/
http://localhost:5012/
http://localhost:5050/


### Deallocate resources
```
docker-compose kill
docker-compose rm
```
