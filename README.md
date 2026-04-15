# AWS Two-Tier Scalable Web Architecture

## Overview
This project demonstrates a highly available and scalable two-tier architecture deployed on AWS.

Architecture:
User → ALB → Auto Scaling Group (EC2 Web Tier) → RDS (Private Database)

---

## Technologies Used
- Amazon VPC
- EC2 (Auto Scaling Group)
- Application Load Balancer
- Amazon RDS (MySQL)
- CloudWatch (Monitoring & Scaling)
- Gemini AI (Cloud architecture diagram)

---

## Architecture Components

### Web Tier (Public)
- EC2 instances in Auto Scaling Group
- Load balanced via ALB
- Hosted in public subnets

### Data Tier (Private)
- MySQL RDS instance
- Hosted in private subnets
- No public access

---

## Features
- High availability across multiple Availability Zones
- Auto Scaling based on CPU utilization
- Secure network segmentation (public vs private)
- Monitoring and alerting with CloudWatch

---

## Testing
- Simulated high CPU usage to trigger scaling
- Verified new instances launch automatically
- Confirmed traffic distribution via ALB

---

## What I Learned
- Designing scalable cloud architectures
- Implementing AWS networking (VPC, subnets, routing)
- Monitoring and automation using CloudWatch
- Building production-like infrastructure

---

## Future Improvements
- Add CI/CD pipeline (GitHub Actions)
- Add HTTPS using ACM
- Deploy a full-stack application
