# Deploy Elastic Search as Stateful-sets into Kubernetes

## Build Elastic Search Image: 

```
$ git clone git@github.com:rajivreddy/elasticseach-kubernetes.git
$ docker build -t elasticsearch:6.3.2 ./es-image/
$ docker push elasticsearch:6.3.2 # push it to Docker registry
```

## Deploy to Kubernetes:  

```
$ kubectl create -f service.yaml
$ kubectl create -f statefulset.yaml
```
