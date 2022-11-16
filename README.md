
# Terraform

Terraform is an infrastructure as code tool.It allows one to define and manage infrastructure resources through human-readable configuration files.

Terraform allows you to use a consistent workflow over your infrastructure lifecycle. The infrastructure as code workflow lets your declaratively manage a variety of services and automate your changes, reducing the risk of human error through manual operations.

## Workflows

In Terraform Cloud, your resources are organized by workspaces.

### The workspaces contain:

- Resource definitions,
- Environment and input variables
- State files.


## Terraform-Docker-Container

## Creating Infrastructure Using Terraform
- Provision an EC2 Instance on AWS

### Prerequisites

- The [Terraform CLI](https://learn.hashicorp.com/tutorials/terraform/install-cli?in=terraform/aws-get-started) installed

- A terraform [Cloud Account](https://app.terraform.io/signup/account?utm_source=learn&_gl=1*39uqcl*_ga*MjUxMTA3NjQ4LjE2NjQxMTMxODU.*_ga_P7S46ZYEKW*MTY2NDMwOTI5MS44LjAuMTY2NDMwOTI5MS4wLjAuMA..) and organisation

- The [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) installed
- [AWS account](https://aws.amazon.com/free/?trk=712ee378-d73b-4293-9bad-8ce09671ea7c&sc_channel=ps&s_kwcid=AL!4422!3!444219541850!e!!g!!aws%20console&ef_id=CjwKCAjw4c-ZBhAEEiwAZ105Rf5wHNi-AEdMfd8_ZPOUaU1CogBX-P7LKUrcX9BouU9QpqwKdLn5HxoCkIQQAvD_BwE:G:s&s_kwcid=AL!4422!3!444219541850!e!!g!!aws%20console) to create resources

- A [Github](https://github.com/) account

- A [git CLI](https://git-scm.com/downloads)

This folder contains the following key files

```README.md``` - Contains documentation

```main.tf``` -  specifies the AWS provider, a provider plugin that Terraform will use to manage your AWS resources. 

```variables.tf``` - defines the input variables 

```outputs.tf``` -  defines the information about your infrastructure that Terraform Cloud will display to you when it makes changes.

```versions.tf```-  defines version constraints for Terraform and the AWS provider and the cloud block for the Terraform Cloud integration.

```terraform.tf```


### Terraform commands
```terraform login``` - to authenticate through terraform cloud

```terraform init``` - run this to initialize the configuration and create your new Cloud Terraform workspace

#### Clone the repository
```
git clone https://github.com/kurves/terraform-docker-container
```
#### cd  into the new directory
```
cd terraform-aws-instance
```
### Initialize the workspace

Initialize the workspace using, initialize backends and install plugins
```
terraform init
```
### apply the configuration

apply the configuration using 
```
terraform apply
```

### Format the configuration
The format command scans the current directory for configuration files 

```
terraform fmt
```
### Validate your configuration
Check your configuration use;
```
terraform validate
```

### Clean up resources
After verifying that the the resources were deployed successfully, clean up using;
```
terraform destroy
```
### Working with modules
use this to install modules
```
terraform get
```
and
```
terraform init
```
