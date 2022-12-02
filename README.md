# azure-resource-group

Create an Azure resource group using Terraform


## Implement the Terraform code
Create a directory in which to test the sample Terraform code and make it the current directory.

Create a file named providers.tf and insert the following 
Create a file named main.tf and insert the following 
Create a file named variables.tf and insert the following
Create a file named outputs.tf and insert the following

## Initialize Terraform
1. `terraform init`
2. `terraform plan -out main.tfplan`
3. `terraform apply main.tfplan`

## Verify the results
`echo "$(terraform output resource_group_name)"`

Azure CLI

`az group show --name <resource_group_name>`

## Clean up resources

1. `terraform plan -destroy -out main.destroy.tfplan`

2. `terraform apply main.destroy.tfplan`
