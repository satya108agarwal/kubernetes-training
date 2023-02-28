# Exercises are provided here to help you confirm all required services are running locally

#### Execute the below command to start the minikube server. This command is tested in mac. Please use the equivalent in windows to start the service
```bash
minikube start 
```

##### Execute below command to check the nodes in cluster

```bash
kubectl get nodes
```

##### Output of the above command show below labels and status should be ready. It's okay to be on different version of kubectl api.
```
Output: 

NAME       STATUS   ROLES           AGE    VERSION
minikube   Ready    control-plane   157d   v1.25.0
```

