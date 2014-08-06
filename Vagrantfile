Vagrant.configure(2) do |config|
  # This is the primary "web" container
  config.vm.define "web" do |web|
    web.vm.network :forwarded_port, guest: 8080, host: 8080
    web.vm.network :private_network, ip: "192.168.50.4"
    web.vm.provider "docker" do |d|
      d.build_dir = "./Docker/web"
      d.ports = ["8080:80"]
    end
  end
end