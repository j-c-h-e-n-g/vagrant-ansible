# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "opscode-ubuntu-14.04" 
  config.vm.synced_folder "./ansible", "/home/vagrant/ansible" 
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "bootstrap.yml"
  end
end
