Vagrant.configure("2") do |config|

  config.vm.define "all_in", primary: true do |all|
    all.vm.box = "qwerty1979/highfive"
    all.vm.hostname = "bananas3"
    all.vm.provision "shell", path: "provision_nginx.sh"
    all.vm.network "private_network", ip: "192.168.56.56"
    all.vm.post_up_message = "All done, enjoy !"
  end

end
