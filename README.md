# Customer Data Processing System on AWS

## Overview

This project demonstrates the design, deployment, and governance of a customer data processing system using AWS cloud services. The solution was built as part of the AWS Cloud Operations course using the AWS Academy Learner Lab environment.

The architecture follows a secure multi-tier design with separated networking, compute, storage, and database layers. The project focuses not only on infrastructure deployment, but also on cloud governance, monitoring, logging, operational visibility, and cost-aware resource management.

---

## Architecture

The environment includes:

- Amazon EC2 instance acting as the processing layer
- Amazon RDS MariaDB instance deployed in private subnets
- Amazon S3 bucket for customer data storage
- Amazon VPC with public and private subnet separation
- Route tables and Internet Gateway configuration
- Security groups for controlled service communication
- Amazon CloudWatch monitoring and dashboards
- Amazon SNS alert notifications
- AWS CloudTrail activity logging

![Architecture](architecture/architecture-diagram.png)

---

## AWS Services Used

### Core Infrastructure
- Amazon EC2
- Amazon RDS (MariaDB)
- Amazon S3
- Amazon VPC
- Route Tables
- Internet Gateway
- Security Groups

### Governance & Operations
- Amazon CloudWatch
- Amazon SNS
- AWS CloudTrail

---

## Phase 1 Implementation

Phase 1 focused on designing and deploying the core AWS infrastructure:

- Multi-tier cloud architecture
- Secure VPC networking
- Public and private subnet deployment
- EC2 and RDS integration
- S3 object storage
- Database connectivity validation
- AWS CLI-based deployment and testing

---

## Phase 2 Governance Features

Phase 2 extended the environment with operational and governance capabilities:

- CloudWatch dashboards and monitoring
- CPU utilization alarms
- SNS email notifications
- CloudTrail activity logging
- Resource tagging strategy
- S3 lifecycle policy for cost optimization

These additions improved operational visibility, governance, auditing, and monitoring within the environment.

---

## Validation

The environment was validated through practical testing:

- SSH connection to EC2 instance
- S3 file upload and retrieval
- Secure EC2-to-RDS database connectivity
- SQL database creation and query execution
- CloudWatch alarm triggering
- SNS email notification delivery
- CloudTrail event verification

---

## Repository Structure

```text
.
├── architecture/       # Architecture diagrams
├── commands/           # AWS CLI and SQL commands
├── docs/               # Troubleshooting knowledge base
├── phase1/             # Phase 1 report
├── phase2/             # Phase 2 report
├── screenshots/        # Validation and implementation evidence
└── README.md

```
---

## Notes

This project was implemented in the AWS Academy Learner Lab environment with temporary sandbox infrastructure, limited IAM permissions, and budget constraints. These limitations required careful resource management, troubleshooting, and cost optimization practices.

---

## Future Improvements

Possible future enhancements include:

- Auto Scaling Groups
- Load Balancer integration
- IAM role-based access control
- Infrastructure as Code (Terraform/OpenTofu)
- Automated backup and recovery strategies
- Enhanced monitoring and security automation

---

## Author

Maab Osman
