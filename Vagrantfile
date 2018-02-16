# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.provider "vmware_workstation" do |vb|
    #vb.gui = true
    vb.memory = "1024"
  end

  config.vm.provision "shell", path: "provision.sh"
end
