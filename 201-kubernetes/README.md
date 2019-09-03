# Azure Virtual Machine Scale Set

## Expected Outcome

In this challenge, you will create a kubernetes cluster, and deploy a service.

The service to deploy is just an  example of how terraform can be used to manage kubernetes resources just like Azure resources.


The resources you will use in this challenge:

- Resource Group
- Virtual Network
- Subnet
- Azure Kubernetes Service (AKS)
- Load Balancer (auto generated)
- Public IP Address (auto generated)

## How to

### Create the base Terraform Configuration

Change directory into a folder specific to this challenge.

For example: `cd ~/TerraformWorkshop/kubernetes/`.

We will start with a few of the basic resources needed.

Create a `main.tf` file to hold our configuration.

### Create Variables

Create a file `variables.tf` and add the following configuration:


### Create Variables TF File

Create a file `terraform.tfvars` and add the following configuration:

### Create Core Infrastructure

Create a file `core.tf` and add the following configuration:



### Run Terraform Workflow

Run `terraform init` since this is the first time we are running Terraform from this directory.

Run `terraform plan` and validate all resources are being created as desired.

Run `terraform apply` and type `yes` when prompted.

Inspect the infrastructure in the portal.

Change the VMSS count to another number and replan, does it match your expectations?

### Clean up

When you are done, run `terraform destroy` to remove everything we created.