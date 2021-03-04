# Docker-container-python
This is building a container from scratch

## Build the Container Yourself and Push to Docker Hub

### Build image
*(If you want to develop yourself)* 
docker build --tag yisongzou/docker_container_python:project2 .

### List docker images
docker image ls

### Run my newly built container

docker run -it project2 python app.py --name "Yisong Zou"

### Push to Docker Hub

*Note:  You will need to change for your Docker Hub Repo*
 docker push yisongzou/docker_container_python:project2

## Run it yourself

```bash
docker pull yisongzou/docker_container_python:project2
docker run -it yisongzou/docker_container_python bash 

#then run python app.py --help
```

## Pass in a command

```bash
docker run -it yisongzou/docker_container_python python app.py --name "Big John"
#the output
Hello Yisong Zou!
```

### More things Do

* Lint the code with Github Actions (see the Makefile)
* Automatically build the container after lint, and push to DockerHub or some other Container Registery



