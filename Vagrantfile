$script = <<SCRIPT
echo "Installing Ruby"
sudo apt-get install ruby1.9.1-dev -y
echo "Installing NodeJS"
sudo apt-get install nodejs -y
echo "Installing Jekyll"
sudo gem install github-pages --no-ri --no-rdoc
# sudo gem install jekyll
date > $HOME/vagrant_provisioned_at
SCRIPT
# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # For a complete reference, see  https://docs.vagrantup.com.

  # boxes at https://atlas.hashicorp.com/search.
  config.vm.box = "ubuntu/trusty64"
  config.vm.box_url = "https://atlas.hashicorp.com/ubuntu/boxes/trusty64"


  # We'll need a way to access our webserver once it's provisioned, so we'll
  # tell Vagrant to forward port 80 from our box to port 8080 on localhost. 
  config.vm.network "forwarded_port", host: 4000, guest: 4000

  # Enable provisioning with an inline shell script. This installs Jekyll.
  config.vm.provision "shell", inline: $script
  
end
