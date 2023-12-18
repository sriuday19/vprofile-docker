Vagrant.configure("2") do |config|
    config.vm.define("docker") do |docker|
        docker.vm.box = "ubuntu/focal64"
        docker.vm.hostname = "docker"
        docker.vm.network "private_network", ip: "192.168.56.25"
    docker.vm.provider "virtualbox" do |vb|
        vb.memory="2048"
    end     
        docker.vm.provision "shell", path: "docker.sh"
    end     
end