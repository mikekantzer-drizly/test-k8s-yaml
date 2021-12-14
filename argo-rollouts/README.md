testing out https://argoproj.github.io/argo-rollouts/

working through https://argoproj.github.io/argo-rollouts/getting-started/

# Setup and Testing
assuming a fresh `minikube` install:
```sh
kubectl create namespace argo-rollouts
kubectl apply -n argo-rollouts -f install.yaml
```

Then, we can hassle around at an app:
```
kubectl apply -f rollout.yaml
kubectl apply -f service.yaml
kubectl argo rollouts get rollout rollouts-demo --watch
```