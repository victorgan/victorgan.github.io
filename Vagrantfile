VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # For a complete reference, see  https://docs.vagrantup.com.

  # boxes at https://atlas.hashicorp.com/search.
  config.vm.box = "ubuntu/trusty64"
  config.vm.box_url = "https://atlas.hashicorp.com/ubuntu/boxes/trusty64"

  # We'll need a way to access our webserver once it's provisioned, so we'll
  # tell Vagrant to forward port 80 from our box to port 8080 on localhost. 
  config.vm.network :forwarded_port, host: 4000, guest: 4000

  # Enable provisioning with an inline shell script. This installs Jekyll.
  config.vm.provision :shell,
    :inline => "sudo apt-get -y install build-essential && sudo /opt/vagrant_ruby/bin/gem install jekyll rdiscount --no-ri --no-rdoc"
  
end
