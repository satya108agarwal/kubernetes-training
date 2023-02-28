# Exercises are provided here to help you become familiar with Kubernetes Pods.

#### Execute below command to create a pod in the cluster
```bash
 kubectl create -f pod.yml
```

#### Execute below command to list all pods 
```bash
kubectl get pods
```

#### Execute below command to describe a pod
```bash
kubectl describe pod frontend
```

#### Execute below command to see the IP of a pod
```bash
kubectl get pods -o wide
```

#### Execute below command to delete the pod
```bash
kubectl delete pod frontend
```
#### Execute below command to check the logs of the workload
```bash
kubectl logs -f frontend
```

#### Execute below command to ssh to the running container to check the contents of the workload or for any troubleshooting
```bash
kubectl exec -it frontend -- /bin/bash
```
# Troubleshoot Pod Failures

##### Execute below command to create a pod which has a image that doesn't exist in container registry.
```bash
 kubectl create -f failed_pod.yml
```

##### Execute below command to check the errors
```bash
 kubectl describe pod imagedoesntexistpod
```

