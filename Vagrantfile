# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # base box
  config.vm.box = "tommartensen/ubuntu-bionic-dev"
  config.vm.box_version = "0.0.1"

  # virtualbox provider configuration: start gui, ram and cpu
  config.vm.provider "virtualbox" do |v|
    v.gui = true
    v.memory = 8192
    v.cpus = 2
  end

  config.vm.provision "ansible_local" do |ansible|
    ansible.install  = true
    ansible.verbose  = true
    ansible.become   = false
    ansible.playbook = "setup_developer_machine.yml"
  end
end
