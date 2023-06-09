# CronJob

### Pre Requisites
* Make sure you have minikube installed
* You should have understanding of deploying a Pod and Job
---
### Example
Start minikube cluster with 2 worker nodes (Optional) 
```bash
minikube start --nodes 3 -p k8s 
```
Check cluster status (Optional) 
```bash
minikube status -p k8s
```
Make sure you are inside CronJob folder
```bash
cd ./example/CronJob
```
Create Namespace and CornJob at same time
```bash
kubectl create -f ./example
```
Switching to k8s-app namespace
```bash
kubectl config set-context --current --namespace=k8s-app 
```
Get CornJob Status
```bash
kubectl get cronjob app-job
```
List Job Status
```bash
kubectl get jobs
```
List pods status
```bash
kubectl get pods
```
Delete Namespace and CornJob at same time
```bash
kubectl delete -f ./example
```
Delete cluster or Clean Up(Optional) 
```bash
minikube delete -p k8s
```

---
### Links
* [Home](https://github.com/vimalmenon/k8s-learn)
* [Previous Topic (Job)](https://github.com/vimalmenon/k8s-learn/tree/master/example/Job)
* [Next Topic (ConfigMap)](https://github.com/vimalmenon/k8s-learn/tree/master/example/ConfigMap)
