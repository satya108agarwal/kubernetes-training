# Exercises are provided here to help you become familiar with Kubernetes Replica Sets.

#### Execute the below command to create a replica set
```bash
 kubectl create -f replicaset.yml
 ```

#### Execute the below command to query replicasets
 ```bash
 kubectl get replicasets
 ```


#### Execute the below command to query pods created by the replicaset
#### Verify the number of pods match to number of replica's mentioned in replica set
```bash
 kubectl get pods
 ```

#### Execute the below command to delete replicasets
   ```bash
kubectl delete replicaset frontend
 ```

##### Execute the below command to check if pods are deleted
```bash
kubectl get pods
 ```