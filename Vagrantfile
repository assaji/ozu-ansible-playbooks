# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "chef-centos6.6"

  config.vm.define :web01 do |web01|
   web01.vm.hostname = "web01"
   web01.vm.network "public_network", ip:"192.168.11.81", :bridge => "en0: Ethernet" 
  end

  config.vm.define :web02 do |web02|
   web02.vm.hostname = "web02"
   web02.vm.network "public_network", ip:"192.168.11.82", :bridge => "en0: Ethernet" 
  end 
 
  config.vm.define :db01 do |db01|
   db01.vm.hostname = "db01"
   db01.vm.network "public_network", ip:"192.168.11.83", :bridge => "en0: Ethernet" 
  end

  config.vm.provider "virtualbox" do |vb|
  #   vb.gui = true
   vb.memory = "512"
  end
  #

end
