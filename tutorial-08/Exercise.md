# Commands to create a NodePort Service

```bash
kubectl create -f configmap.yml

# ssh into the container and printenv all environment variables

kubectl exec -it pod/pod-env-var -- /bin/sh

```

```bash

printenv # command to print all environment variables set from configmap

keys=image.public.key=771
rsa.public.key=42
database_uri=mongodb://localhost:27017
HOSTNAME=pod-env-var
database=mongodb
```