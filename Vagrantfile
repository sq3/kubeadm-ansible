# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "bento/ubuntu-20.04"
  config.vm.hostname = "node-0"
  config.vm.network "private_network", type: "dhcp"
  config.vm.network :private_network, ip: "172.28.128.6"
  config.vm.hostname = "node-0.dev.xyz.com.de"
  config.hostsupdater.aliases = ["node-0.dev.xyz.com.de"]
  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"va
  config.vm.provider "virtualbox" do |v|
    v.name = "node-0"
    v.linked_clone = true
    v.memory = "4096"
    v.cpus = 2
  end
end
