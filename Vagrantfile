# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box_url = ""
  config.vm.box = "Palo-FW"
  config.vm.boot_timeout = 600
  config.vm.network "forwarded_port", guest: 443, host: 4434
  config.ssh.insert_key = false
  config.vm.synced_folder '.', '/vagrant', disabled: true
  config.vm.provider :virtualbox do |vb|
    vb.name = 'Palo-Lab'
  end
end
