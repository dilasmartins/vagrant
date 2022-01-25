Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"
    config.disksize.size = '30GB'
    config.vm.network "private_network", ip: "192.168.5.11"
    config.vm.hostname = "centos"
    config.vm.provision "ansible", playbook: "playbook.yml"
    config.vm.provider "virtualbox" do |vb|
        vb.memory = "4096"
        vb.cpus = "2"
    end
end

