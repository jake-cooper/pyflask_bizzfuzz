# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "hashicorp/precise32"
  config.vm.box_check_update = true
  config.vm.network "forwarded_port", guest: 5000, host: 5000
# config.vm.synced_folder "../data", "/vagrant_data"

  config.vm.provision "shell", inline: <<-SHELL
     sudo apt-get -qqy update
     sudo 
apt-get -qqy install python-flask
     sudo apt-get -qqy install python-pip
     sudo pip install requests

   vagrantTip="[35m[1mThe shared directory is located at /vagrant\nTo access your shared files: cd /vagrant(B[m"
echo -e $vagrantTip > /etc/motd

   SHELL
end
