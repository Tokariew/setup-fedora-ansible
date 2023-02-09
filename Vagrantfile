Vagrant.configure("2") do |config|
  config.vm.box = "fedora/37-cloud-base"
  config.ssh.insert_key = false
  config.vm.provider "libvirt" do |v|
    v.memory = 1536
    v.cpus = 2
  end
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
