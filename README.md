## Dev and Engineering sandbox environments in Azure

Use this jetpack to jump start your vnet in Azure to configure your sandbox dev / engineering environment.  Create your Azure account (local personal subscription) and use azure cloud cli bash or powershell to turn the ignition on your environment.  First, ensure you are not connected to any mastery klusters or vnets.  Git clone the files to your local directory and use the appropriate commands to construct and deconstruct your environments.  

## Please refer to Tier2Support_cmd for command reference and answers.txt for more details on each step
1.  Ensure Azure Cloud CLI is setup in your Azure cloud console

2.  Create a VM in Azure (vcpu x 2, 8 mb ram)

3a.  Install Docker (Ubuntu dependencies)

3b.  Install Docker Engine

4.  Install Prometheus

5.  Create simple infrastructures with Azure Cloud CLI using terraform 
