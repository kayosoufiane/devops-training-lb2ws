# DevOps Training - Load balancing of 2 web servers - Practical / Usage - using Docker compose

## 1 - Clone the repository locally
```
git clone https://github.com/ykandrirody/devops-training-lb2ws.git
```


## 2 - Start all services

```
cd devops-training-lb2ws

docker-compose up -d
```

## 3 - Test web servers :
```
http://localhost:5011/   Will be up.
http://localhost:5012/   will be up.
http://localhost:5050/   Alternate between : Version A, Version B
```

## 4 - Stop the web server A
```
docker kill mywebserver.a
```

## 5 - Test web servers :
```
http://localhost:5011/   Will be down !
http://localhost:5012/   Will be up.
http://localhost:5050/   Only : Version B 
```

## 6 - Deallocate resources
```
docker-compose kill
docker-compose rm
```
