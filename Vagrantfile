VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(2) do |config|
  
  config.vm.box = "williamyeh/ubuntu-trusty64-docker"
  config.vm.network "private_network", ip: "192.168.50.101"
  config.vm.hostname = "vagrant-docker-example"

  config.vm.provision :docker
  config.vm.provision "shell", path:"provision.sh"
  config.vm.provision :docker_compose, compose_version:"1.9.0"
  #config.vm.provision "shell", path:"provision2.sh"   se puede poner en marcha el servicio autmáticamente o manualmente desde /vagrant/service 
  # con docker-compose up 
 
end