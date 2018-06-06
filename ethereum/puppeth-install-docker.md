# puppeth docker installation instructions

Ubuntu
``` 
$ sudo apt-get update
$ sudo apt-key adv --keyserver hkp://p80.pool.sks-keyservers.net:80--recv-keys 58118E89F3A912897C070ADBF76221572C52609D
$ sudo apt-add-repository 'deb https://apt.dockerproject.org/repoubuntu-xenial main' 
$ sudo apt-get update
$ sudo apt-cache policy docker-engine
$ sudo apt-get install -y docker-engine
$ sudo systemctl status docker
$ sudo usermod -aG docker $(whoami)
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.11.2/docker-compose-Linux-x86_64" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose 
$ sudo reboot 
```
 
