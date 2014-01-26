Vagrant.configure("2") do |config|
  config.vm.box = "saucy64"
  config.vm.box_url = "http://uec-images.ubuntu.com/vagrant/saucy/current/saucy-server-cloudimg-amd64-vagrant-disk1.box"
  config.vm.provision "docker",
    images: ["ubuntu"]
  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.customize ["modifyvm", :id, "--cpuexecutioncap", "50"]
  end
end
