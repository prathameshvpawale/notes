# docker_notes
## version information
``` 
docker -v 
```
## run container
``` 
docker run -it ubuntu
```
## running container
``` 
docker container ls
```
``` 
docker ps
```
## all container
``` 
docker container ls -a
```
``` 
docker ps -a
```
## Stopping a Container
``` 
docker stop CONTAINER_ID
```
``` 
docker kill CONTAINER_ID
```
## Live Shell
``` 
docker exec -it CONTAINER_ID /bin/sh
```
``` 
docker start -ai CONTAINER_ID
```