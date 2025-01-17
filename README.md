# Terraform IaC for WebJob Storage trigger


This Terraform configuration creates the following resources in Azure:

- Storage Account: A general-purpose v2 storage account with a specified name and location.
- Web App: An Azure Web App with the specified name, runtime stack (e.g., .NET), and location.
- Application Settings: Sets the AzureWebJobsStorage connection string as an environment variable in the Web App, allowing the WebJob to access the Storage Account.

## Prerequisites:

1. Azure Subscription: You need an active Azure subscription.
2. Terraform: Install and configure Terraform on your local machine.
3. Azure CLI: Install and configure the Azure CLI to authenticate with your subscription.

## Usage:

1. Create a new directory for your Terraform project and place the main.tf and providers.tf files inside it.
2. Initialize Terraform: Run `terraform init` to initialize the working directory and download necessary providers.
3. Plan the changes: Run `terraform plan` to preview the infrastructure changes that will be made.
4. Apply the changes: Run `terraform apply` to create the resources in Azure.
5. Deploy your WebJob: Deploy your compiled WebJob to the created Web App.
