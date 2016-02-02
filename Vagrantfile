Vagrant.configure(2) do |config|
  config.vm.box = "centOS_6.7"
   config.vm.network "forwarded_port", guest: 80, host: 8080  # make sure that these ports are free on your host machine
   config.vm.network "forwarded_port", guest: 8080, host: 8080
   config.vm.network "forwarded_port", guest: 443, host: 443
   config.vm.network "forwarded_port", guest: 22, host: 2222
   config.vm.network "public_network" # you can change to "private_name" 
   config.vm.provider "virtualbox" do |vb|
     vb.memory = "4096"  # change memory accordingly
   end
end
