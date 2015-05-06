# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
	config.vm.define "kibana" do |kibana|
		kibana.vm.hostname = "kibana"
		kibana.vm.box = "hashicorp/precise64"
		kibana.vm.provision :ansible do |ansible|
			ansible.playbook = "test.yml"
		end
		kibana.vm.network "private_network", ip: "192.168.50.24"
	end
end
