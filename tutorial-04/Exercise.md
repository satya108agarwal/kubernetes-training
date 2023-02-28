# Commands to create a ReplicaSet

```bash
# command to create a replica set
 kubectl create -f replicaset.yml
 ```

 ```bash
# command to query replicasets
 kubectl get replicasets
 ```

  ```bash
# command to query pods created by the replicaset
# check if 3 instances of pod exist
 kubectl get pods
 ```

   ```bash
# command to delete replicaset
kubectl delete replicaset frontend
 ```

    ```bash
# command to check if pods are deleted
kubectl get po
 ```