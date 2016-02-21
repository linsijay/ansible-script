Vagrant.configure(2) do |config|
  config.vm.box = "debian/jessie64"
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.sudo = true
  end
   
  config.vm.provider "virtualbox" do |v|
    v.cpus = 2
  end
   
end
