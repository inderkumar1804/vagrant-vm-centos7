# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|

	config.vm.define "mytstsrv1" do |mytstsrv1|
    		mytstsrv1.vm.box = "centos/7"
    		mytstsrv1.vm.hostname = "mytstsrv1.example.com"
    		mytstsrv1.vm.network "private_network", ip: "172.42.42.100"
    		mytstsrv1.vm.provider "virtualbox" do |v|
      		  v.name = "mytstsrv1"
      		  v.memory = 2048
      		  v.cpus = 2
      		# Prevent VirtualBox from interfering with host audio stack
      		  v.customize ["modifyvm", :id, "--audio", "none"]
    		end
  	end
end
