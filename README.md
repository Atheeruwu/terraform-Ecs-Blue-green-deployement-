ECS Blue-Green Deployment with Terraform
Overview

This project demonstrates how to implement blue-green deployment for containerized applications on AWS ECS using Terraform.
The goal is to achieve zero-downtime deployments, safe traffic switching, and fully reproducible infrastructure using Infrastructure as Code.

Architecture

Amazon ECS (Fargate)

Application Load Balancer (ALB)

Target Groups (Blue / Green)

Amazon ECR

VPC, Subnets, Security Groups

IAM Roles & Policies

Terraform Modules

Traffic is routed through an Application Load Balancer, allowing seamless switching between blue and green environments during deployments.

Key Features

Blue-green deployment strategy for ECS services

Zero-downtime application updates

Infrastructure provisioned entirely with Terraform

Modular and reusable Terraform configuration

Clear separation of environments (blue & green)

Safe rollback capability by switching target groups

What I Implemented

Designed ECS task definitions and services for blue and green environments

Configured ALB listeners and target groups for traffic shifting

Provisioned AWS infrastructure using Terraform (VPC, ECS, ALB, IAM, ECR)

Implemented Terraform variables and modules for flexibility and reuse

Ensured idempotent and repeatable deployments using IaC best practices

Technologies Used

Cloud: AWS (ECS, ALB, ECR, IAM, VPC)

Infrastructure as Code: Terraform

Containers: Docker

Version Control: Git, GitHub

How This Project Demonstrates DevOps Skills

Practical understanding of blue-green deployment strategies

Hands-on experience with AWS ECS and Fargate

Strong foundation in Terraform and Infrastructure as Code

Knowledge of load balancing, traffic routing, and rollback strategies

Focus on automation, reliability, and deployment safety

Use Case

This setup is suitable for production environments where:

Zero downtime is required during deployments

Safe rollback is critical

Infrastructure needs to be versioned and reproducible
