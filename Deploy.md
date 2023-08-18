# GooSM Kubernetes how to Deploy tutorial

Bu tutorial goosm product'ı için hazırlanmıştır.

```
curl -LO https://github.com/umutderebek/kubernetes/blob/main/goosm-deployment.yaml
```
```
curl -LO https://github.com/umutderebek/kubernetes/blob/main/mysql-deployment.yaml
```
```
curl -LO https://github.com/umutderebek/kubernetes/blob/main/kustomization.yaml
```

1-) After that you should check kustomization file for resources. Contains all the resources for deploying a goo and a MySQL database. You can apply the directory by

```
kubectl apply -k ./
```

2-) Now we should verify our secrets and Pvc's ( Persistent Volumes)
```
kubectl get pvc
```

3-) you can check runing services

You can see all pods with the code below

```
kubectl get po -A
```



