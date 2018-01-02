# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.synced_folder ENV['ANSIBLE_HOME'], "/home/vagrant/ansible"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "bootstrap.yml"
  end
end
