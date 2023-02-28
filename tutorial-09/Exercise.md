# Exercises are provided here to help you become familiar with Kubernetes secrets.

#### Below command executes the secret
```bash
kubectl create -f secret.yml
```

#### Command to list all secrets
```bash
 kubectl get secrets
```


#### Command to update the secret 
```bash
kubectl edit secret/newsecret -o yaml
```