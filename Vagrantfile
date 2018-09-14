Vagrant.configure("2") do |config|
  config.vm.box = "qwerty1979/highfive"
  config.vm.hostname = "bananas3"
  config.vm.provision "shell", path: "provision_nginx.sh"
  config.vm.network "private_network", ip: "192.168.56.56"
end
