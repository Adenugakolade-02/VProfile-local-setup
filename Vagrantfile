Vagrant.configure("2") do |config|
	config.hostmanager.enabled = true
	config.hostmanager.manage_host = true
	
	config.vm.define "webo1" do |web01|
		web01.vm.box = "ubuntu/bionic64"
		web01.vm.hostname = "web01"
		web01.vm.network "private_network", ip: "192.168.33.11"
	end
	
	config.vm.define "app01" do |app01|
		app01.vm.box = "geerlingguy/centos7"
		app01.vm.hostname = "app01"
		app01.vm.network "private_network", ip: "192.168.33.12"
	end
	
	config.vm.define "rmq01" do |rmq01|
		rmq01.vm.box = "geerlingguy/centos7"
		rmq01.vm.hostname = "rmq01"
		rmq01.vm.network "private_network", ip: "192.168.33.16"
	end
	
	config.vm.define "mc01" do |mc01|
		mc01.vm.box = "geerlingguy/centos7"
		mc01.vm.hostname = "mc01"
		mc01.vm.network "private_network", ip: "192.168.33.14"
	end
	
	config.vm.define "db01" do |db01|
		db01.vm.box = "geerlingguy/centos7"
		db01.vm.hostname = "db01"
		db01.vm.network "private_network", ip: "192.168.33.15"
	end
end