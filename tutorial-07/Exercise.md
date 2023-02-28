# Commands to create a NodePort Service

```bash
kubectl create -f service.yml

# see the status of the service and deployment using the following command
kubectl get all
```

```bash

# launch the service 
minikube service nginx-service

# above command is tested on Mac, please find the equivalent in Windows to launch the service in browser.
```