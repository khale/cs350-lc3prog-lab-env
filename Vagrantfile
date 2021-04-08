Vagrant.configure("2") do |config|

  config.vm.box = "mrlesmithjr/bionic64-desktop"
  config.vm.synced_folder ".", "/home/vagrant/lab3"
  config.vm.provision :shell, path: "https://gist.githubusercontent.com/khale/bd7387ea00d9de1917e4ab357afc4617/raw/fd91cd60df380f1fd81dfb33da0df88c9d566832/lc3-bootstrap.sh"

  config.vm.provider "vmware_desktop" do |v|
    v.gui = true
  end

  config.vm.provider "virtualbox" do |v|
    v.gui = true
  end

end
