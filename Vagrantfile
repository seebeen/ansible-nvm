# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "hashicorp/xenial64"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "test.yml"
  end
end
