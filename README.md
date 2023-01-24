# wcs-terraform

Contains a solution for the Terraform assignment. This is intended to be run on an EC2 instance with a role that allows it to create other instances.

## Installation

1. Copy the files to the instance.
2. [Install Terraform on the instance](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli#install-terraform).
3. Run `terraform init`
4. *Optional*: Run `terraform validate` and `terraform plan` to do a simple static check of the configuration validity.
5. Run `terraform apply` and confirm.
6. Take note of the output. You'll see a line noting the public IP of the new server, for example: `Webserver-Public-IP = 3.237.82.153`

## Validation

After Terraform applies the configuration, you should be able to visit the IP noted above via HTTP and see the test message "My Test Website With Help From Terraform Provisioner".
