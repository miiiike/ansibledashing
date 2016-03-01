# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname = "dashingansiblebase"    

  config.vm.synced_folder "./dashing", "/home/vagrant/dashing"

  config.vm.network "public_network", bridge: "en0: Wi-Fi (AirPort)", ip: 
  "10.169.13.155", netmask: "255.255.0.0"

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
    end
end