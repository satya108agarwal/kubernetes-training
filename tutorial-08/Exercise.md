# Commands to create a ConfigMap

```bash
kubectl create -f configmap.yml

# ssh into the container and printenv all environment variables
kubectl exec -it pod/pod-env-var -- /bin/sh

```

```bash
# command to print all environment variables set from configmap
printenv 

Output:

keys=image.public.key=771
rsa.public.key=42
database_uri=mongodb://localhost:27017
HOSTNAME=pod-env-var
database=mongodb
```