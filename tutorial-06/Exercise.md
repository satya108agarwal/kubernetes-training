# Commands to check the status of the deployment

```bash
kubectl rollout status deployment/nginx-deployment

# see the status of the deployment

```


```bash
kubectl rollout history deployment/nginx-deployment

# see the history of all the revisions

```


```bash
kubectl rollout undo deployment/nginx-deployment

# go back to previous state

```

```bash
kubectl rollout undo deployment/nginx-deployment

# go back to previous state

```
```bash
kubectl rollout undo deployment/nginx-deployment --to-revision=0

# go back to any previous state, specify the previous revision number

```

```bash
kubectl rollout status deployment/nginx-deployment

# see the status of the deployment

```

```bash
kubectl rollout history deployment/nginx-deployment

# see the history of all the revisions

```