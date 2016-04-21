# -*- mode: ruby -*-
# vi: set ft=ruby :

system("
    if [ #{ARGV[0]} = 'up' ] && [ -f './requirements.yml' ] ; then
        echo 'You are doing vagrant up, updating from requirements.yml'
        ansible-galaxy install -r requirements.yml --force
    fi
")

VAGRANT_VERSION = 2
Vagrant.configure(VAGRANT_VERSION) do |config|
	config.vm.define "aws-credentials" do |server|
		server.vm.box = "hashicorp/precise64"
		server.vm.hostname = "aws-credentials"
		server.vm.provision :ansible do |ansible|
			ansible.playbook = "test.yml"
		end
	end
end
