This is where I throw YAML for testing stuff in a local minikube.

```
minikube start
minikube addons enable metrics-server
minikube addons enable ingress
```

using `kind`:
```
kind create cluster --config=kind-config.yaml
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml
```

