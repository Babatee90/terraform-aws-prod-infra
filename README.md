# terraform-aws-prod-infra

## Overview
This repository demonstrates a **production-style Terraform AWS infrastructure** using a
**parent (root) module with reusable child modules**.

It is designed as a **DevOps portfolio project** to showcase:
- Infrastructure as Code (IaC)
- Modular Terraform design
- AWS networking fundamentals
- Secure and scalable patterns suitable for real-world environments

The infrastructure provisions:
- A VPC with a public subnet
- Internet Gateway and routing
- Security Group with controlled access
- EC2 instance running Nginx via user_data

---

## Repository Structure
terraform-aws-prod-infra/
├── modules/
│ ├── vpc/ # VPC, subnet, routing
│ └── ec2/ # EC2 instance and security group
├── envs/
│ └── dev/ # Root (parent) module
├── .gitignore
└── README.md

- **modules/** contains reusable child modules
- **envs/dev/** is the root module where Terraform is executed

---

## Architecture
Internet
|
[ Internet Gateway ]
|
[ Public Subnet ]
|
[ EC2 Instance (Nginx) ]


---

## Tech Stack
- **Terraform** (>= 1.5)
- **AWS**
  - VPC
  - EC2
  - Security Groups
  - Internet Gateway

---

## How to Deploy

### Prerequisites
- AWS account
- AWS CLI configured:
  ```bash

  terraform init
terraform plan
terraform apply

## Author

 Babatola Adeniyi
GitHub: https://github.com/Babatee90  

  aws configure

