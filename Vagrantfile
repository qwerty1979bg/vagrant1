Vagrant.configure("2") do |config|

  config.vm.define "own_box", autostart:false do |own|
    own.vm.box = "qwerty1979/highfive"
    own.vm.post_up_message = "task: 'Use your own box from Vagrant Cloud'"
  end

  config.vm.define "bananas3", autostart:false do |banana|
    banana.vm.box = "qwerty1979/highfive"
    banana.vm.hostname = "bananas3"
    banana.vm.post_up_message = "task: 'hostname to bananas3'"
  end

  config.vm.define "nginx", autostart:false do |nginx|
    nginx.vm.box = "qwerty1979/highfive"
    nginx.vm.provision "shell", path: "provision_nginx.sh"
    nginx.vm.post_up_message = "task: 'script to install nginx'"
  end

  config.vm.define "ip", autostart:false do |ip|
    ip.vm.box = "qwerty1979/highfive"
    ip.vm.network "private_network", ip: "192.168.56.56"
    ip.vm.post_up_message = "task: 'set ip to 192.168.56.56'"
  end

  config.vm.define "all_in", primary: true do |all|
    all.vm.box = "qwerty1979/highfive"
    all.vm.hostname = "bananas3"
    all.vm.provision "shell", path: "provision_nginx.sh"
    all.vm.network "private_network", ip: "192.168.56.56"
    all.vm.post_up_message = "All done, enjoy !"
  end

end
