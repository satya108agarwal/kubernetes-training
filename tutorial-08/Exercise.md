# Exercises are provided here to help you become familiar with Kubernetes Config Map.


#### Execute the below command to create a ConfigMap
```bash
kubectl create -f configmap.yml
```

#### ssh into the container and printenv all environment variables
```bash
kubectl exec -it pod/pod-env-var -- /bin/sh
```

#### command to print all environment variables set from configmap
```bash
printenv 
```

#### Output of above command should contain the following environment variables
```
Output:

keys=image.public.key=771
rsa.public.key=42
database_uri=mongodb://localhost:27017
HOSTNAME=pod-env-var
database=mongodb
```