# Terraform Module: AWS EC2 Instance with Docker

This Terraform module provisions an AWS EC2 instance with the latest Amazon Linux 2023 AMI and installs Docker on it.

## Usage

```hcl
provider "aws" {
  region = "us-east-1"
}

module "docker_instance" {
    source   = "<github-username>/docker-instance/aws"
    key_name = "example"
}
