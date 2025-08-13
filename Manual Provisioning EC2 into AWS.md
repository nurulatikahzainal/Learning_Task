# Steps to Manually Provision EC2 into AWS using Terraform

## Install Terraform
1. Go to the [Terraform Downloads](https://developer.hashicorp.com/terraform/downloads) page.
2. Download the package for your operating system.
3. Extract and place the Terraform binary in a directory included in your system `PATH`(in the Environment Variable).
4. Verify installation using command prompt: terraform --version

## Install AWS CLI (with latest version)
1. Go to the [AWS CLI Downloads](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) page.
2. Download the version for your operating system.
3. Verify installation using command prompt: aws --version

## Configure AWS CLI Credential
1. Create AWS account (will create a root user account with free version).
2. Create IAM user account.
3. Crate permission for the IAM user account
4. Create Access Key (Access Key ID and Secret Access Key will be created and need to copy once provided as it will not be fetchable again)
5. Configure AWS through command prompt by providing the following:
   1. AWS Access Key ID
   2. AWS Secret Access Key
   3. Default region (e.g., ap-southeast-1)
   4. Output format (e.g., json)

