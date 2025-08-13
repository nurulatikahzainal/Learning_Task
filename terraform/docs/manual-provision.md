# Steps to Manually Provision EC2 into AWS using Terraform

## Install Terraform
1. Go to the [Terraform Downloads](https://developer.hashicorp.com/terraform/downloads) page.
2. Download the package for your operating system.
3. Extract and place the Terraform binary in a directory included in your system `PATH`(in the Environment Variable).
4. Verify installation using command prompt: terraform --version.

## Install AWS CLI (with latest version)
1. Go to the [AWS CLI Downloads](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) page.
2. Download the version for your operating system.
3. Verify installation using command prompt: aws --version

## Configure AWS CLI Credential
1. Create AWS account (will create a root user account with free version).
2. Create IAM user account.
3. Crate permission for the IAM user account.
4. Create Access Key (Access Key ID and Secret Access Key will be created and need to copy once provided as it will not be fetchable again).
5. Configure AWS through command prompt by providing the following:
   1. AWS Access Key ID
   2. AWS Secret Access Key
   3. Default region (e.g., ap-southeast-1)
   4. Output format (e.g., json)
6. Verify configuration using command prompt: aws sts get-caller-identity.

## Create Terraform Project Structure
1. Run in command prompt 'mkdir Learn-Terraform-Get-Started-AWS' to create a new folder.
2. Create [terraform.tf](https://github.com/nurulatikahzainal/Learning_Task/blob/development/terraform/docs/terraformtf%20code.md).
3. Create [main.tf](https://github.com/nurulatikahzainal/Learning_Task/blob/development/terraform/docs/maintf%20code.md).
4. Put the tf file created into Learn-Terraform-Get-Started-AWS folder.
5. Run command prompt 'terraform fmt' to format the tf files according to Harshicorp recommended style.

## Provisioning
1. Initialize Terraform workspace by running in command prompt 'terraform init'.
2. Validate the terraform either the configuration is valid or not by runningin command prompt as 'terraform validate'.
3. Once valid, run in command prompt as 'terraform apply' to plan and apply the configuration to indicate the terraform will create the EC2 instance.
4. Inspect the state file by running in command prompt as 'terraform state list'.
5. Once validated, destroy the EC2 by running in command prompt as 'terraform destroy' to kill the run.


