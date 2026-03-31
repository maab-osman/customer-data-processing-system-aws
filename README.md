# Customer Data Processing System AWS
## Overview
This project demonstrates the design and deployment of a customer data processing system using AWS. The architecture follows a multi-tier design with secure networking and service integration.

## Architecture

The system consists of:

- Amazon EC2 (processing layer)
- Amazon RDS (database layer)
- Amazon S3 (object storage)
- VPC with public and private subnets
- Internet Gateway and route tables
- Security groups for controlled access
  
![Architecture](architecture/architecture-diagram.png)

## Key Features
- Secure communication between EC2 and RDS
- Private database deployment
- File storage using S3
- CLI-based deployment and validation
- SQL-based data processing

## Validation
The system was validated by:

- Connecting to EC2 via SSH
- Uploading data to S3
- Connecting to RDS from EC2
- Creating and querying a customer database

## Project Structure

- `Phase1_Report.pdf` → Full report
- `architecture/` → Architecture diagram
- `screenshots/` → Implementation evidence
- `commands/` → CLI commands used

## Notes
This project was implemented in the AWS Academy Learner Lab environment with limited permissions and budget constraints.

## Author
Maab Osman
