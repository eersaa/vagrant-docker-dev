Vagrant.configure("2") do |config|
  config.vm.define "dev"
  config.vm.hostname = "dev"
  config.vm.box = "ubuntu/jammy64"
  config.vm.provider "virtualbox" do |vb|
    vb.cpus = 1
    vb.memory = 1024
  end

  config.vm.provision "shell", path: "vagrant-scripts/bootstrap.sh", privileged: false

end
