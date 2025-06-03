Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-22.04"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
    vb.cpus = 2
  end

  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt update
    sudo apt install -y software-properties-common
    sudo apt-add-repository --yes --update ppa:ansible/ansible
    sudo apt install -y ansible
  SHELL

  config.vm.provision "ansible_local" do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.become = true
  end
end
