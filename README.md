# Parsec Terraform

This repository contains the terraform code to depoly a Parsec Gaming instance to AWS. 

To get started clone this repo!

# Requirements
  - Before you begin, make sure the Parsec Client is installed on your computer.
  - Ensure you have [AWS] and [Terraform] installed.
  
# Configuring AWS 

  - Create an AWS IAM  user and create Access keys. [AWS IAM Documentation]
  - Once created, ensure you have your credentials defined in ~/.aws/credentials

```
[AWS-User]
aws_access_key_id = insert_key_here
aws_secret_access_key = insert_key_here
```

  - Create a security group named parsec-security-group. [Security Group Documentation] with the below configuration. 
  - parsec-security-group should have these ports 8000-8011 TCP and UDP are open.

[AWS IAM User Documentation]: <https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html>
[Terraform]: <https://www.terraform.io/intro/getting-started/install.html>
[AWS]: <https://docs.aws.amazon.com/cli/latest/userguide/installing.html>
[Security Group Documentation]: <https://docs.aws.amazon.com/AmazonVPC/latest/UserGuide/VPC_SecurityGroups.html#CreatingSecurityGroups>
