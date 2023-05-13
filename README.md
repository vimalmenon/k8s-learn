# Learning K8S


### Kubectl command

### Minikube command
Start minikube with cluster
```
minikube start -n <number of nodes> -p <cluster-name>
``` 
Status of the cluster
```
minikube status -p <cluster-name>
```
Add worker nodes
```
minikube node add --worker -p <cluster-name>
```
Delete worker nodes
```
minikube node delete <node-name> -p <cluster-name>
```
Delete all the cluster
```
minikube delete --all
```