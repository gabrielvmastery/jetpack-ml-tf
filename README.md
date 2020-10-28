## Dev and Engineering sandbox environments in Azure

Use this jetpack to jump start your vnet in Azure to configure your sandbox dev / engineering environment.  Create your Azure account (local personal subscription) and use azure cloud cli bash or powershell to turn the ignition on your environment.  First, ensure you are not connected to any mastery klusters or vnets.  Git clone the files to your local directory and use the appropriate commands to construct and deconstruct your environments.  

##Please refer to Tier2Support_cmd for command reference and footnotes in description for more details on each step
1.  Ensure Azure Cloud CLI is setup in your Azure cloud console
## See 1a footnote

2.  Create a VM in Azure (vcpu x 2, 8 mb ram)

3.  Install Docker (Ubuntu dependencies):
sudo apt-get update

sudo apt-get install \
    apt-transport-https \
    ca-certificates \
    curl \
    gnupg-agent \
    software-properties-common
	
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo apt-key fingerprint 0EBFCD88

sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"

Install Docker Engine: 
sudo apt-get update
sudo apt-get install docker-ce docker-ce-cli containerd.io

4.  Install Prometheus:
## See 4a footnote
Download exe at prometheus.io
tar xvfz prometheus-*.tar.gz
cd prometheus-*
./prometheus --config.file=prometheus.yml

5.  Create simple infrastructures with Azure Cloud CLI using terraform 
