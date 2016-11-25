# -*- mode: ruby -*-
# vi: set ft=ruby :

$script = <<BASH
sudo apt-get update
sudo apt-get install -y python-dev python-pip libffi-dev
sudo pip install ansible
BASH

Vagrant.configure(2) do |config|
  config.vm.box = "opscode-ubuntu-14.04" 
  config.vm.provision "shell", inline: $script
end
