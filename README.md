## Components needed
- `brew instal kubectl`
- `brew install minikube`
- `brew install hyperkit`
> ### *If using Apple Chip
Follow this [link](https://docs.docker.com/desktop/kubernetes/) to use Docker-Desktop instead

## How to Deploy 
***Always apply config and secret before making deployment**
```
kubectl apply -f <CONFIG_NAME>.yaml
kubectl apply -f <SECRET_NAME>.yaml
kubectl apply -f <DEPLOYMENT_NAME>.yaml
```

## Visit WebApp
1. If using minikube

Find the IP by using cli below:
- `minikube ip` 
- `kubectl get node -o wide`

2. If using Docker Desktop
- visit `localhost:<EXPOSED_PORT>`

****There are cases you will hit with memory issue on deployment, try raise the docker desktop ram to resolve it**