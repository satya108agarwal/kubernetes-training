# Exercises are provided here to help you become familiar with Kubernetes Deployments.

#### Execute below command to create a deployment
```bash
 kubectl create -f deployment.yml
```

#### Execute belowcommand to list all the resources created at once
```bash
kubectl get all
```

#### Execute below command to list all pods
```bash
kubectl get pods
```

#### Notes: Deployment created 3 pods since the replicas requested are 3. Id's may differ from system to system because they are randomly generated.
```

pod/nginx-deployment-7fb96c846b-b2jl9   1/1     Running   0          10s
pod/nginx-deployment-7fb96c846b-f2nsb   1/1     Running   0          10s
pod/nginx-deployment-7fb96c846b-t5x5p   1/1     Running   0          10s
```

####  Execute the below command to scale the deployment
```bash
kubectl scale --replicas=4 deployment/nginx-deployment
```

#### Execute the below command to update the container image in deployment
```bash
kubectl set image deployment.v1.apps/nginx-deployment nginx=nginx:1.16.1
```

#### Check in watch mode that updates happen in rolling recycle manner so there is no downtime to the end user. 
```bash
watch kubectl get pods
```


#### Execute the below command and edit the image version to 1.15.1
#### Check the output in watch mode that updates happen in rolling recycle manner, End result is no downtime to the end user
```bash
kubectl edit deployment/nginx-deployment
```

