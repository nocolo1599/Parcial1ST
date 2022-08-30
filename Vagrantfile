
Vagrant.configure("2") do |config|
  if Vagrant.has_plugin? "vagrant-vbguest"
    config.vbguest.no_install = true
    config.vbguest.auto_update = false
    config.vbguest.no_remote = true
  end
  config.vm.define :servidor1 do |servidor1|
    servidor1.vm.box = "centos/stream8"
    servidor1.vm.network :private_network, ip: "192.168.50.4"
    servidor1.vm.hostname = "servidor1"
  end

  config.vm.define :servidor2 do |servidor2|
    servidor2.vm.box = "centos/stream8"
    servidor2.vm.network :private_network, ip: "192.168.50.5"
    servidor2.vm.hostname = "servidor2"
  end
end

