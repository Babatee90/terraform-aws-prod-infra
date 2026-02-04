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
