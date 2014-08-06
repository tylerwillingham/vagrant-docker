Vagrant.configure(2) do |config|
  config.vm.provider "docker" do |d|
    d.build_dir = "./Docker/web"
  end
  config.vm.network :forwarded_port, host: 4567, guest: 80
end