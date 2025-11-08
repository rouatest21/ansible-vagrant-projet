Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/jammy64"
  config.vm.hostname = "ansible-vm"
  config.vm.network "private_network", ip: "192.168.56.10"

  # Synchronise le dossier local "ansible" avec la VM
  config.vm.synced_folder "./ansible", "/home/vagrant/ansible"

  # Installe Ansible dans la VM
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt update -y
    sudo apt install -y ansible
  SHELL
end
