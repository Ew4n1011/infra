Vagrant.require_version ">= 2.2.2"

Vagrant.configure(2) do |config|
  config.vm.define "infra-test" do
    config.vm.box = "bento/ubuntu-22.04"
    config.vm.network "private_network", ip: "172.30.1.5"
    config.ssh.insert_key = true

    config.vm.provision "ansible_local" do |ansible|
      ansible.compatibility_mode = "2.0"
      ansible.galaxy_role_file = "requirements.yml"
      ansible.inventory_path = "tests/inventories/integration_testing/inventory"
      ansible.playbook = "infra.yml"
      ansible.become = true
    end
  end
end