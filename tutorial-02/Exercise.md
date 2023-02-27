# Commands to create, describe and delete the pods

```bash
# command to create a pod in the cluster
 kubectl create -f pod.yml

```

```bash
# command to list all pods 
kubectl get pods
```


```bash
# command to describe a pod
kubectl describe pod frontend
```

```bash
# command to see the IP of a pod
kubectl get pods -o wide
```

```bash
# command to delete the pod
kubectl delete pod frontend
```

```bash
# command to check the logs of the workload
kubectl logs -f frontend
```

```bash
# command to login to the running container to check the contents of the workload
kubectl exec -it frontend -- /bin/bash
```
# Troubleshoot Pod Failures

```bash
# command to create a pod which has a image that doesn't exist
 kubectl create -f failed_pod.yml
```

```bash
# use describe command to check the errors
 kubectl describe pod imagedoesntexistpod

```

