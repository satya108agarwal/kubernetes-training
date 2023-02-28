# Commands to create, update and scale a Deployment via yaml file

```bash
# command to create a deployment
 kubectl create -f deployment.yml
```

```bash
# command to list all the resources created
kubectl get all

# Deployment create a replicaset and pods
```


```bash
# command to list all pods
kubectl get pods

# Deployment created 3 pods since the replicas requested are 3
pod/nginx-deployment-7fb96c846b-b2jl9   1/1     Running   0          10s
pod/nginx-deployment-7fb96c846b-f2nsb   1/1     Running   0          10s
pod/nginx-deployment-7fb96c846b-t5x5p   1/1     Running   0          10s
```

```bash
# Scale the deployment

kubectl scale --replicas=4 deployment/nginx-deployment
```

```bash
# Update the deployment
kubectl set image deployment.v1.apps/nginx-deployment nginx=nginx:1.16.1

# see in watch mode that updates happen in rolling recycle manner so there is no downtime to the end user

watch kubectl get pods
```

```bash
kubectl edit deployment/nginx-deployment

# set the image version to 1.15.1
# see in watch mode that updates happen in rolling recycle manner so there is no downtime to the end user
```

