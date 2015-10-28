# vagrant-docker
A Vagrant VM have docker and docker compose installed ready to roll

### Prerequisites

Vagrant: http://www.vagrantup.com/downloads

### How to use? 
1) git clone git@github.com:richardhe-awin/vagrant-docker.git   

2) Uncomment the following line and replace with your path to mount a directory
```
#  config.vm.synced_folder "{path on your local machine}", "{path on the vagrant box}"
```

3) Uncomment the following line and replace with your private docker hub to get around the insecure registry issue
```
#  echo 'DOCKER_OPTS="$DOCKER_OPTS --insecure-registry={your private docker hub host name}:5000"' | sudo tee -a /etc/default/docker
```

4) run `vagrant up` to start provisioning the VM
5) run `vagrant ssh` to start using the virtual machine
