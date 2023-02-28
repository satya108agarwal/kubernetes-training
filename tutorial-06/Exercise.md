# Exercises are provided here to help you become familiar with Kubernetes Deployment Rollbacks.


#### To Check the status of the deployment
```bash
kubectl rollout status deployment/nginx-deployment
```


#### To Check  the history of all the revisions
```bash
kubectl rollout history deployment/nginx-deployment
```


#### Revert back to previous state
```bash
kubectl rollout undo deployment/nginx-deployment
```

#### To go back to any previous state, specify the previous revision number
```bash
kubectl rollout undo deployment/nginx-deployment --to-revision=0
```
#### To Check the status of the deployment
```bash
kubectl rollout status deployment/nginx-deployment
```

#### To Check  the history of all the revisions
```bash
kubectl rollout history deployment/nginx-deployment
```