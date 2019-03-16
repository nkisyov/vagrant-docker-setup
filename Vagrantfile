# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.define "template-vm" 
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
    v.name = "template"
    v.gui = false
  end
  config.vm.network "private_network", ip: "192.168.101.101"
  config.vm.network "forwarded_port", guest: 8080, host: 8080
  config.vm.synced_folder "./source/", "/source/", owner: "www-data", group: "www-data"
  config.vm.provision :shell, :path => "provision.sh"
 end
 