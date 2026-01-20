# ECS Blue-Green Deployment with Terraform

## Overview
This repository demonstrates a **blue-green deployment strategy** for containerized applications on **AWS ECS (Fargate)** using **Terraform**.  
The setup enables **zero-downtime deployments** by switching traffic between two identical environments (blue and green) behind an Application Load Balancer.

All infrastructure is provisioned using **Infrastructure as Code (IaC)**, ensuring repeatable, version-controlled, and production-ready deployments.

---

## Architecture
- Amazon ECS (Fargate)
- Application Load Balancer (ALB)
- Blue & Green Target Groups
- Amazon ECR
- VPC, Subnets, Security Groups
- IAM Roles and Policies
- Terraform (modular configuration)

Traffic is routed through the ALB, allowing safe traffic switching between environments during deployments.

---

## Features
- Blue-green deployment strategy on ECS
- Zero-downtime application updates
- Infrastructure fully provisioned with Terraform
- Modular and reusable Terraform code
- Safe rollback by switching target groups
- Cloud-native AWS architecture

---

## Implementation Details
- Defined ECS task definitions and services for blue and green environments
- Configured ALB listeners and target groups for controlled traffic routing
- Provisioned AWS resources (VPC, ECS, ALB, IAM, ECR) using Terraform
- Used Terraform variables and modules for flexibility and reusability
- Followed Infrastructure as Code best practices for idempotent deployments

---

## Technologies Used
- **AWS:** ECS (Fargate), ALB, ECR, IAM, VPC
- **Infrastructure as Code:** Terraform
- **Containers:** Docker
- **Version Control:** Git, GitHub

---

## Use Case
This project is suitable for environments where:
- High availability is required
- Application downtime must be avoided during deployments
- Rollback needs to be fast and reliable
- Infrastructure must be reproducible and version-controlled

---

## Future Enhancements
- CI/CD integration using GitHub Actions or Jenkins
- Monitoring and logging with CloudWatch or Prometheus
- Canary deployment support
- Multi-environment setup (dev, staging, production)

---

## Repository Purpose
This project was created to practice and demonstrate real-world DevOps deployment patterns using AWS and Terraform.
