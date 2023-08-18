# GooSM Kubernetes how to Deploy tutorial

Bu tutorial goosm product'ı için hazırlanmıştır.

```
curl -LO https://github.com/umutderebek/kubernetes/blob/main/goosm-deployment.yaml
```
```
curl -LO https://k8s.io/examples/application/wordpress/mysql-deployment.yaml
```

After that you should check kustomization file for resources. Contains all the resources for deploying a goo and a MySQL database. You can apply the directory by

```
kubectl apply -k ./
```
