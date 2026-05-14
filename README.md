# Customer Data Processing System on AWS

## Overview
This project demonstrates the design, deployment, and governance of a customer data processing system using AWS cloud services. The architecture follows a secure multi-tier design that separates networking, compute, storage, and database resources across public and private subnets.

The project was implemented as part of the AWS Cloud Operations course using the AWS Academy Learner Lab environment.

## Architecture

The system architecture includes:

- Amazon EC2 instance acting as the processing layer
- Amazon RDS MariaDB instance deployed in private subnets
- Amazon S3 bucket for customer data storage
- Amazon VPC with public and private subnet separation
- Internet Gateway and route tables for controlled connectivity
- Security groups for secure communication between services
- CloudWatch monitoring and dashboards
- SNS alert notifications
- CloudTrail activity logging

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

## Phase 1 Features

Phase 1 focused on designing and deploying the core infrastructure:

- Multi-tier AWS architecture
- Secure VPC networking
- Public and private subnet deployment
- EC2 and RDS integration
- S3 object storage
- Database connectivity validation
- CLI-based deployment and testing

---

## Phase 2 Governance Features

The environment was extended with operational and governance capabilities including:

- Amazon CloudWatch dashboards and alarms
- Amazon SNS alert notifications
- AWS CloudTrail activity logging
- Resource tagging strategy
- S3 lifecycle policies for storage cost optimization

These additions improved monitoring, auditing, operational visibility, and governance within the AWS environment.

---

## Validation

The environment was validated through practical testing:

- SSH connection to EC2 instance
- S3 file upload and retrieval
- Secure connection from EC2 to RDS
- SQL database creation and query execution
- CloudWatch alarm triggering
- SNS email notification delivery
- CloudTrail event logging verification

---

## Repository Structure

```text
architecture/     → Architecture diagrams
commands/         → AWS CLI commands and validation steps
phase1/           → Phase 1 report
phase2/           → Phase 2 report
screenshots/      → Implementation and validation evidence
```

---

## Notes

This project was implemented in the AWS Academy Learner Lab environment with temporary sandbox infrastructure, limited permissions, and budget constraints. The environment required careful cost optimization and resource management practices.

---

## Future Enhancements

Possible future improvements include:

- Auto Scaling Groups
- Load Balancer integration
- IAM role-based access control
- Automated backups and recovery
- Infrastructure as Code (Terraform/OpenTofu)
- Enhanced monitoring and security automation

---

## Author

Maab Osman
