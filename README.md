<<<<<<< HEAD
# vpc-module
=======
# Terraform VPC Module

This Terraform module creates a basic VPC setup on AWS, including:
- A custom VPC
- One public subnet
- An Internet Gateway
- A Route Table with default route
- Route Table association

---

## 🏗️ Module Usage

```hcl
module "vpc" {
  source             = "git::https://github.com/Akshay5119/vpc-module.git?ref=main"
  vpc_cidr           = "10.0.0.0/16"
  public_subnet_cidr = "10.0.1.0/24"
  availability_zone  = "ap-south-1a"
  vpc_name           = "terraform-demo-vpc"
}
>>>>>>> c19b0f8 (Initial commit for VPC module)
