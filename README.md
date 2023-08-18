# GooSM Kubernetes how to use tutorial

Bu tutorial goosm product'ı için hazırlanmıştır.

--
goosm
--

## Install dependencies for docker

```
sudo apt update
```
```
sudo apt install apt-transport-https ca-certificates curl software-properties-common -y
```

```
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
```

```
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
```

```
apt-cache policy docker-ce
```

```
sudo apt install docker-ce -y
```

```
sudo systemctl status docker
```

## Install dependencies for kubernetes

```
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
```

```
curl -LO "https://dl.k8s.io/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"
```

```
echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check
```
if validated result is : OK you can continue.

```
sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
```
install kubectl and we'd giving some permissions.
```
chmod +x kubectl
mkdir -p ~/.local/bin
mv ./kubectl ~/.local/bin/kubectl
```

```
kubectl version --client
```
if kubectl version gives our installation is successed.

## Install dependencies for Minikube

```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

```
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube
```

