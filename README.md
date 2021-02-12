# Exemple simple-webapp pour docker et Kubernetes
## commandes de base
```shell
git clone https://github.com/system-dev-formations/simple-webapp.git
cd simple-webapp/
docker build -t simple-webapp .
docker images
docker run -d --name web simple-webapp 
docker logs web
docker rm -f web
docker run -d --name web -p 5000:5000 simple-webapp 
docker ps
docker images
k create -f simple-webapp.yaml 
k get pod
docker login
docker image tag simple-webapp systemdevformations/simple-webapp
docker images
docker push systemdevformations/simple-webapp
```
