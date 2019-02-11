# Installing Docker on Linux server

1.Update packages
```sh 
yum update -y
```
2.Install docker
```sh 
yum install docker -y
```

# Docker Installation on CentOS/Redhat server
### docker will not support on Centos 6.5 version as same as Redhat as well. Please install 6.5 version and above.
##### Referance URL : https://docs.docker.com/install/linux/docker-ce/centos/#install-using-the-repository
### PREREQUISITES

Please follow below steps to install docker CE on CentoOS server instance. For RedHat only Docker EE available 

1.Install required packages.

 
sudo yum install -y yum-utils \
  device-mapper-persistent-data \
  lvm2
  
2.Use the following command to set up the stable repository.
 
 
 sudo yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo


### INSTALLING DOCKER CE

1.Install the latest version of Docker CE.
 
sudo yum install docker-ce


2.Start Docker.
 
sudo systemctl start docker


3.Verify that docker is installed correctly by running the hello-world image.

sudo docker run hello-world

