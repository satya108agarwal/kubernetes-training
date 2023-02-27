# Commands to create with resource request and limits defined

```bash
# command to create a pod in the cluster
# cpu :200m translates to 2 virtual or physical cpu cores 
 kubectl create -f pod.yml

```
# Nginx worload not ready to serve the traffic because /ready end point returns 404.

```bash
# command to create a pod in the cluster which is never ready
 kubectl create -f nginx-not-ready.yml

```

```bash
# command to create a pod in the cluster which is never ready
 kubectl create -f nginx-not-ready.yml

```

```bash
# check the error message for the workload to see what went wrong
 kubectl describe po nginx-not-ready

 ```