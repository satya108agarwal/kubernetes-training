# Exercises are provided here to help you become familiar with Kubernetes Node Port Service.


#### Below command creates the NodePort Service
```bash
kubectl create -f service.yml
```

#### See the status of the service and deployment using the following command
```bash
kubectl get all
```

#### launch the service 
```bash
minikube service nginx-service
```

#### Above command is tested on Mac, please find the equivalent in Windows to launch the service in browser.