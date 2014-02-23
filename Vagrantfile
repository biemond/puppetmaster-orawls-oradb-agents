# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  config.vm.define "adminwls" , primary: true do |admin|
    admin.vm.box = "centos-6.5-x86_64"
    admin.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    admin.vm.hostname = "adminwls.example.com"

    admin.vm.network :private_network, ip: "10.10.10.20"
  
    admin.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1200"]
      vb.customize ["modifyvm", :id, "--name", "adminwls"]
    end
  
  end

  config.vm.define "adminwls2" , primary: true do |admin|
    admin.vm.box = "centos-6.5-x86_64"
    admin.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    admin.vm.hostname = "adminwls2.example.com"

    admin.vm.network :private_network, ip: "10.10.10.21"
  
    admin.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1200"]
      vb.customize ["modifyvm", :id, "--name", "adminwls2"]
    end
  
  end

  config.vm.define "adminwls3" , primary: true do |admin|
    admin.vm.box = "centos-6.5-x86_64"
    admin.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    admin.vm.hostname = "adminwls3.example.com"

    admin.vm.network :private_network, ip: "10.10.10.22"
  
    admin.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1200"]
      vb.customize ["modifyvm", :id, "--name", "adminwls3"]
    end
  
  end

  config.vm.define "adminwls4" , primary: true do |admin|
    admin.vm.box = "centos-6.5-x86_64"
    admin.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    admin.vm.hostname = "adminwls4.example.com"

    admin.vm.network :private_network, ip: "10.10.10.23"
  
    admin.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "3500"]
      vb.customize ["modifyvm", :id, "--name", "adminwls4"]
    end
  
  end

  config.vm.define "adminwls5" , primary: true do |admin|
    admin.vm.box = "centos-6.5-x86_64"
    admin.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    admin.vm.hostname = "adminwls5.example.com"

    admin.vm.network :private_network, ip: "10.10.10.24"
  
    admin.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "2500"]
      vb.customize ["modifyvm", :id, "--name", "adminwls5"]
    end
  
  end
  
  config.vm.define "nodewls1" do |node1|

    node1.vm.box = "centos-6.5-x86_64"
    node1.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"
  
    node1.vm.hostname = "nodewls1.example.com"

    node1.vm.network :private_network, ip: "10.10.10.100"
  
    node1.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1024"]
      vb.customize ["modifyvm", :id, "--name", "nodewls1"]
    end

  end

  config.vm.define "nodewls2" do |node2|

    node2.vm.box = "centos-6.5-x86_64"
    node2.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    node2.vm.hostname = "nodewls2.example.com"

    node2.vm.network :private_network, ip: "10.10.10.200", auto_correct: true
  
    node2.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "1024"]
      vb.customize ["modifyvm", :id, "--name", "nodewls2"]
    end
  
  end

  config.vm.define "oradb" , primary: true do |oradb|
    oradb.vm.box = "centos-6.5-x86_64"
    oradb.vm.box_url = "https://dl.dropboxusercontent.com/s/np39xdpw05wfmv4/centos-6.5-x86_64.box"

    oradb.vm.hostname = "oradb.example.com"
    oradb.vm.network :private_network, ip: "10.10.10.5"
  
    oradb.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm"     , :id, "--memory", "2000"]
      vb.customize ["modifyvm"     , :id, "--name"  , "oradb"]
    end

  end  


end
