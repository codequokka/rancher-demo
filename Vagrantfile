# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu2004"

  # Rancher server
  config.vm.define "rancher01" do |server|
    server.vm.hostname = "rancher01"
    server.vm.network "private_network", ip: "192.168.33.11"
    server.vm.provider "virtualbox" do |vb|
      vb.cpus = 1
      vb.memory = 4096
    end
  end

  # K8s clusters
  config.vm.define "cluster01" do |server|
    server.vm.hostname = "cluster01"
    server.vm.network "private_network", ip: "192.168.33.21"
    server.vm.provider "virtualbox" do |vb|
      vb.cpus = 6
      vb.memory = 6144
    end
  end

  config.vm.define "cluster02" do |server|
    server.vm.hostname = "cluster02"
    server.vm.network "private_network", ip: "192.168.33.22"
    server.vm.provider "virtualbox" do |vb|
      vb.cpus = 6
      vb.memory = 6144
    end
  end
end