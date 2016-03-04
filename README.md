# DevOps Training - Load balancing of 2 web servers - Practical - using Docker compose


## Usage

### Clone the repository locally
```
git clone https://github.com/ykandrirody/devops-training-lb2ws.git
```


### Start all services

```
cd devops-training-lb2ws

docker-compose up -d
```

### Test web servers :
```
http://localhost:5011/   Will be up.
http://localhost:5012/   will be up.
http://localhost:5050/   Alternate between : Version A, Version B
```

### Stop the web server A
```
docker kill mywebserver.a
```

### Test web servers :
```
http://localhost:5011/   Will be down !
http://localhost:5012/   Will be up.
http://localhost:5050/   Only : Version B 
```

### Deallocate resources
```
docker-compose kill
docker-compose rm
```
