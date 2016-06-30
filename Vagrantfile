# Defines our Vagrant environment
#
# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

 # create maven node (change this to new project)

  config.vm.define :maven do |maven_config|
      maven_config.vm.box = "bento/centos-6.7"
      maven_config.vm.hostname = "maven"
      maven_config.vm.network :private_network, ip: "192.168.1.29"
      maven_config.vm.provider "virtualbox" do |vb|
      end 
      maven_config.vm.provision :shell, path: "bootstrap.sh", privileged: false
  end 

end
