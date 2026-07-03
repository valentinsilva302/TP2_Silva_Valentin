Vagrant.configure("2") do |config|
  # Sistema operativo
  config.vm.box = "ubuntu/jammy64"
  config.vm.hostname = "VMPruebas2"
  
  # Red
  # config.vm.network "private_network", ip: "192.168.56.3"

  # Discos nuevos (como pide el TP)
  config.vm.disk :disk, size: "5GB", name: "extra_storage"
  config.vm.disk :disk, size: "2GB", name: "extra_storage2"

  # Configuración de VirtualBox
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.name = "VMPruebas2"
    vb.cpus = 2
    vb.linked_clone = true
  end
end
