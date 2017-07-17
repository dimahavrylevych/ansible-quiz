Vagrant.configure("2") do |config|
  config.ssh.insert_key = false

  config.vm.define "web1" do |web|
    web.vm.box = "centos/7"
  	web.vm.network "private_network", ip: "192.168.61.3"
  	web.vm.hostname = "web1.mentorship"
  end

  config.vm.define "web2" do |web|
    web.vm.box = "centos/7"
    web.vm.network "private_network", ip: "192.168.61.4"
  	web.vm.hostname = "web2.mentorship"
  end

  config.vm.define "db1" do |db|
    db.vm.box = "ubuntu/trusty64"
    db.vm.network "private_network", ip: "192.168.61.5"
  	db.vm.hostname = "db1.mentorship"
  end

  config.vm.define "proxy" do |proxy|
    proxy.vm.box = "centos/7"
    proxy.vm.network "private_network", ip: "192.168.61.6"
  	proxy.vm.hostname = "proxy.mentorship"
  end

end
