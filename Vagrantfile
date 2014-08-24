VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.network "forwarded_port", guest: 4000, host: 4000

  config.vm.provision "shell", path: "provision/install-node"
  config.vm.provision "shell", path: "provision/install-jekyll"
end
