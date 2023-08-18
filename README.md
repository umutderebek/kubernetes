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



## Install dependencies via Composer

```
composer update
```
