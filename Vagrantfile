# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"
ENV['VAGRANT_DEFAULT_PROVIDER'] = 'virtualbox'
HOST_IP = '192.168.56.65'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
config.vm.define "ansible1" do |ansible1|
ansible1.vm.hostname = "ansible1.rnstech.com"
ansible1.vm.box = "bento/centos-7.2"
ansible1.vm.box_url = "bento/cento-7.2"
ansible1.vm.network :private_network,
      ip: HOST_IP,
      netmask: '255.255.255.0'
end

config.vm.define "ansible2" do |ansible2|
ansible2.vm.hostname = "ansible2.rnstech.com"
ansible2.vm.box = "bento/centos-7.2"
ansible2.vm.box_url = "bento/centos-7.2"
ansible2.vm.network :private_network,
      ip: '192.168.56.66',
      netmask: '255.255.255.0'
end

end