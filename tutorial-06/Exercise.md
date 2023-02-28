# Commands to check the status of the deployment

```bash
# see the status of the deployment
kubectl rollout status deployment/nginx-deployment
```


```bash
# see the history of all the revisions
kubectl rollout history deployment/nginx-deployment
```


```bash
# revert back to previous state
kubectl rollout undo deployment/nginx-deployment
```

```bash
# revert back to previous state
kubectl rollout undo deployment/nginx-deployment
```

```bash
# go back to any previous state, specify the previous revision number
kubectl rollout undo deployment/nginx-deployment --to-revision=0
```

```bash
# see the status of the deployment
kubectl rollout status deployment/nginx-deployment
```

```bash
# see the history of all the revisions
kubectl rollout history deployment/nginx-deployment
```