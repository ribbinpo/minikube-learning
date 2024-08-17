# Minikube Learning

This is learn component of Kubernetes with Minikube.

In this learning is consist of 2 parts:
1. mongodb
2. webapp

Minikube Command
```bash
# check ip
minikube ip
```

Kubectl Command
```bash
# check ip
kubectl get node -o wide

# run kubernets components
kubectl apply -f mongo-config.yaml
kubectl apply -f mongo-secret.yaml
kubectl apply -f mongo.yaml
kubectl apply -f webapp.yaml

# get all components in cluster
kubectl get all

# configmap, secret, pod, svc
kubectl get configmap
kubectl get secret
kubectl get pod

# describe format: kubectl describe [component] [name]
kubectl describe service webapp-service

# view logs of containers
kubectl logs name... -f
```