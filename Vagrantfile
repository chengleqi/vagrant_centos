# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.hostname = "centos"
  config.vm.box = "centos/7"
  config.ssh.insert_key = false
  config.vm.network "private_network", ip: "192.168.56.10"
  config.vm.provider "virtualbox" do |vb|
    vb.cpus = 8
    vb.memory = "2048"
  end
  config.vm.provision "file", source: "~/.ssh/id_ed25519.pub", destination: "~/.ssh/id_ed25519.pub"
  config.vm.provision "shell", inline: "cat ~/.ssh/id_ed25519.pub >> ~/.ssh/authorized_keys", privileged: false
  config.vm.provision "shell", path: "bootstrap.sh"
end
