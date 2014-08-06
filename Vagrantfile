Vagrant.configure(2) do |config|
  # This is the primary "web" container
  config.vm.define "web" do |web|
    web.vm.provider "docker" do |d|
      d.build_dir = "./Docker/web"
    end
  end
end