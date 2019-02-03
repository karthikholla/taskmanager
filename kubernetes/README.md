## Install on Mac
```
curl -Lo minikube https://storage.googleapis.com/minikube/releases/v0.33.1/minikube-darwin-amd64 && chmod +x minikube && sudo mv minikube /usr/local/bin/
```

## Deploy the clusters

### Syntax

kubectl create -f <deployment.yml>

```
kubectl create -f ingress/nginx.yml

kubectl create -f database/db.yml

kubectl create -f application/endpoint.yml
kubectl create -f application/scheduler.yml

```

## Scale out
```
kubectl scale deployment <deploymentname> --replicas=<no. of replicas>
```
