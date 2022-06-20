Vagrant.configure(2) do |config|
  config.vm.box = "debian/contrib-stretch64"
  config.vm.box_version = "9.9.0"
  config.vm.provider "virtualbox" do |vb|
    vb.name = "debian"
    vb.memory = "2079"
    vb.cpus = 2
    end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
