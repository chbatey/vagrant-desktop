# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.host_name = "desktop"
  config.vm.network :private_network, ip: "192.168.10.220"

#  config.vm.provision :ansible do |ansible|
#    ansible.playbook = "provisioning/playbook.yml"
#  end

  config.vm.provider :virtualbox do |vb|
    vb.customize ["modifyvm", :id, "--memory", "2024"]
    vb.gui = true
  end
end
