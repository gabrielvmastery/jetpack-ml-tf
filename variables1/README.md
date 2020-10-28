# Create a VM using variables.tf and providing cmd line arg for username and password

terraform apply -var 'admin_username=plankton' -var 'admin_password=Password1234'

git push origin master
