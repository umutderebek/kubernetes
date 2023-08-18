# GooSM Kubernetes how to Deploy tutorial


1-) Files in the repository create files with the same name and copy their contents. After that you should check kustomization file for resources. Contains all the resources for deploying a goo and a MySQL database. You can apply the directory by

```
kubectl apply -k ./
```

2-) Now we should verify our secrets and Pvc's ( Persistent Volumes)
```
kubectl get secrets
```

```
kubectl get pvc
```

3-) you can check runing services

You can see all pods with the code below

```
kubectl get po -A
```

4-) This containers names can be changed anyway , if you want to enter your container's you can use below this code 

```
kubectl exec -it demo-pod -- /bin/sh
```

5-) your folder ls/var/www/html you can deploy your webprojects

```
minikube service --all
```

Enjoy



