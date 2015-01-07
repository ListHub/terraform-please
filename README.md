# Terraform Please

Uses [Terraform](http://www.terraform.io/). It creates multiple CoreOS nodes, and installs [Shipyard](http://www.shipyard-project.com).

This was originally based on [Terraform-Demo](https://github.com/funkymonkeymonk/terraform-demo)

To run:
 - Create file tf/terraform.tfvars the files in the tf directory or use environment variables to set these keys.
 - You will need to set the following variables either in a terraform.tfvars file or via the commandline:
```
# EC2 Variables
access_key = "YOUR_ACCESS_KEY"
secret_key = "YOUR_SECRET_KEY"
subnet_id = "YOUR_SUBNET"
vpc_id = "YOUR_VPC"
token = "TOKEN_FROM_discovery.etcd.io/new"
aws_key_name = "YOUR_SSH_KEYNAME"
```
 - Install [Terraform](https://www.terraform.io/downloads.html)
 - Install [FleetCtl](https://github.com/coreos/fleet/releases)
 - Run init.sh
 - Copy and run the last output line "export FLEETCTL..."
 - Run add_engine.sh
