# Configuring Remote State in Terraform

This task involves transitioning from a local Terraform state file to using a remote state backend in Azure Blob Storage. This setup is essential for collaborative infrastructure management, ensuring that the state is safely stored and accessible by the entire team.

## Prerequisites

- Basic understanding of Terraform and Azure.
- Terraform installed on your machine.
- Azure CLI installed and configured.

## Hands-on Task

1. Fork this repository.
2. Set Up Local Backend.
    * Ensure your initial `main.tf` file includes a basic setup for the local backend.
    * Initialize Terraform to use the local backend.
3. Transition to Remote State Backend.
    * Modify your `main.tf` to configure the remote backend in Azure.
    * Create necessary Azure resources for the backend configuration.
    * Apply the configuration to create the necessary Azure resources.
    * Initialize Terraform with the new backend configuration, migrating the state from local to remote.
4. Verify the Remote State Configuration.
    * Run Terraform plan and apply commands to verify the setup.
    * Check the Azure Blob Storage to ensure the `terraform.tfstate` file is stored there.