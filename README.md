# k8s-kustomize-airflow

Projeto para utilizar k8S com airflow com CI/CD.

alias k='kubectl'
alias kns='kubectl config set-context --current --namespace'

kubectl create namespace ingress-nginx
kubectl create namespace airflow

kubectl config set-context --current --namespace=ingress-nginx

kns ingress-nginx

ingress-nginx

```
kind create cluster --name airflow-ingress --config kind-ingress.yaml
k get nodes

kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/main/deploy/static/provider/kind/deploy.yaml
```

dentro do path do airflow:


```
kustomize build . --enable-helm | kubectl apply -f -
```