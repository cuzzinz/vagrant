Vagrant.configure("2") do |config|

  config.vm.define "pmast" do |pmast|
    pmast.vm.box = "centos65"
    pmast.vm.hostname = "pmast"
    pmast.vm.network "private_network", ip: "172.16.0.100"
    pmast.vm.network :forwarded_port, host: 8099, guest: 3000

    config.vm.provider "virtualbox" do |v|
      v.memory = 1526
    end

  end

  config.vm.define "node1" do |node1|
    node1.vm.box = "centos65"
    node1.vm.hostname = "node1"
    node1.vm.network "private_network", ip: "172.16.0.101"
  end

#  config.vm.define "node2" do |node2|
#    node2.vm.box = "centos65"
#    node2.vm.hostname = "node2"
#    node2.vm.network "private_network", ip: "172.16.0.102"
#  end

end
