# install virtualbox
## documents
https://www.virtualbox.org/wiki/Linux_Downloads
## add repository to /etc/apt/sources.list

## add apt-key

## apt-get update and apt-get install

## trouble shoot
### set proxy
https://www.quora.com/How-do-I-set-the-proxy-setting-using-Linux-command-line-on-Ubuntu-14-04
### proxy setting doesn't affect 
source  /etc/environment

# install Install kubectl
## install dependency apt-transport-https
## add repository to /etc/apt/sources.list.d/kubernetes.list
## apt-get update and apt-get install kubectl

# install Install Minikube
## document 
https://github.com/kubernetes/minikube/releases

# no proxy settings
in the file /etc/environment,  add 127.0.{1..255}.{1..255},192.168.{1..255}.{1..255} in the no_proxy  
## Sample:  
no_proxy="localhost,127.0.0.1,127.0.{1..255}.{1..255},192.168.{1..255}.{1..255}"

after change, run source /etc/environment
