# DevOps Training - Load balancing of 2 web servers - Practical - using Docker compose


## Usage

### Start all services

```
cd devops-lb2ws-training

docker-compose up -d
```

### Stop the web server A
```
docker kill mywebserver.a
```

### Deallocate resources
```
docker-compose kill
docker-compose rm
```
