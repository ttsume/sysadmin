Vagrant.configure(2) do |config|
  config.vm.box = "debian/contrib-stretch64"
  config.vm.box_version = "9.9.0"
  config.vm.hostname = "debian-test"
  config.vm.network "public_network", ip: "192.168.66.222", hostname: true
  config.vm.provider "virtualbox" do |vb|
    vb.name = "debian"
    vb.memory = "2048"
    vb.cpus = 2
    #vb.gui = true
    end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
