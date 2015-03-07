# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "chef-centos6.6"
  config.vm.network "public_network", :bridge => "en0: Ethernet"
  
  config.vm.define :web01
  config.vm.define :web02
  config.vm.define :db01

  config.vm.provider "virtualbox" do |vb|
  #   vb.gui = true
     vb.memory = "512"
   end
  #

end
