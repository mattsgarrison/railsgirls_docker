Vagrant.configure("2") do |config|
  config.vm.box = "saucy64"
  config.vm.provision "docker" do |d|
    d.pull_images "ubuntu"
    d.pull_images "mattsgarrison/railsgirls-docker"
    d.run "ubuntu",
      cmd: "bash -l"
      #args: "-v '/vagrant:/var/www'"
  end

  config.vm.provider "virtualbox" do |v|
    v.memory = 1024
    v.customize ["modifyvm", :id, "--cpuexecutioncap", "50"]
  end
end
