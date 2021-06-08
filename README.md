# Steps to make a vagrant file, launch a VM and install nginx
- Go to the location of the 'Vagrantfile', put followingh lines of code:
'Vagrant.configure("2") do |config|' and 'config.vm.box = "ubuntu/xenial64"', this creates the virtual machine
- 'vagrant up' starts the virtual machine 
- 'vagrant status' tells us if the virtual box is running
- 'vagrant ssh' = Vagrant will go into into this instance of the machine without the instance name
- 'sudo apt-get update -y' updates virtual machine
- 'sudo apt-get upgrade -y' upgrades virtual machine
- 'exit' logs out of the virtual machine
- 'config.vm.network "private_network", ip: "192.168.10.100"' creates ip for virtual machine, this is added to the Vagrantfile
- 'vagrant destroy' destroys the virtual machine associated with the Vagrantfile 
- 'vagrant reload' reloads the virtual machine

sudo id for admin access

# Installing nginx
'sudo apt-get install nginx' installs nginx
