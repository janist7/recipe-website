# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network :forwarded_port, guest: 5000, host: 8000
  config.vm.provision "shell", path: "add_variables.sh", privileged: false
  config.vm.provision "shell", path: "setup.sh"
end