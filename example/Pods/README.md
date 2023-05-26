# Pods

### Pre Requisites
* Please make sure you have minikube installed

### Example
Make sure you have minikube cluster started with 2 worker nodes
```bash
minikube start -nodes 3 -p k8s
```
Check cluster status
```bash
minikube status -p k8s
```
Make sure you are inside Pods folder
```bash
cd ./example/Pods
```
Create a Pod
```bash
kubectl apply -f ./example/01-Pods.yaml 
```
Check Pod status
```bash
kubectl get pods
```
Get Pod in detail
```bash
kubectl describe pods frontend-app-pods
```
---
### Links
* [Home](https://github.com/vimalmenon/k8s-frontend)
* [Previous Topic (K8S Architecture)](https://github.com/vimalmenon/k8s-learn/tree/master/example/K8S%20Architecture)
* [Next Topic (Pods)](https://github.com/vimalmenon/k8s-learn/tree/master/example/Pods)