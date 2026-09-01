# Terraform AWS VPC Module

A reusable Terraform module to provision a basic AWS VPC with public and private subnets, an internet gateway, and route tables.

## What this creates
- A VPC with a configurable CIDR block
- Public and private subnets across multiple Availability Zones
- An Internet Gateway attached to the VPC
- Route tables for public subnet internet access

## Usage
```hcl
module "vpc" {
  source     = "./"
  vpc_cidr   = "10.0.0.0/16"
  aws_region = "us-east-1"
}
```

## Tech
- Terraform
- AWS (VPC, EC2 networking)

## About
Built to demonstrate Infrastructure-as-Code practices used in production environments for provisioning repeatable, version-controlled cloud infrastructure.
