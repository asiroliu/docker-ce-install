refer to [https://docs.docker.com/v17.09/engine/installation/linux/docker-ce/ubuntu/#prerequisites](https://docs.docker.com/v17.09/engine/installation/linux/docker-ce/ubuntu/#prerequisites)

* Artful 17.10 (Docker CE 17.11 Edge and higher only)
* Zesty 17.04
* Xenial 16.04 (LTS)
* Trusty 14.04 (LTS)

# install
```terminal
sudo apt-get remove docker docker-engine docker.io
sudo apt-get update
sudo apt-get install -y apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo apt-key fingerprint 0EBFCD88
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"
sudo apt-get update
sudo apt-get install docker-ce
sudo systemctl start docker
```

# uninstall
```terminal
sudo apt-get purge docker-ce
sudo rm -rf /var/lib/docker
```
