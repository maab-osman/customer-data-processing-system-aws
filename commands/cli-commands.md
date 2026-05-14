# AWS CLI and Database Commands

## Connect to EC2 Instance

```bash
ssh -i labsuser.pem ec2-user@<EC2-PUBLIC-IP>
```

---

## Install MariaDB Client on EC2

```bash
sudo dnf install -y mariadb105
```

---

## Connect to RDS Database

```bash
mysql -h <RDS-ENDPOINT> -u admin --ssl -p
```

---

## Create Database

```sql
CREATE DATABASE customer_data;
USE customer_data;
```

---

## Create Customers Table

```sql
CREATE TABLE customers (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100)
);
```

---

## Insert Sample Data

```sql
INSERT INTO customers (name, email)
VALUES
('Alice', 'alice@email.com'),
('Bob', 'bob@email.com'),
('Sara', 'sara@email.com');
```

---

## Query Customer Data

```sql
SELECT * FROM customers;
```

---

## Upload File to Amazon S3

```bash
aws s3 cp customers.csv s3://maab-customer-data-processing/
```

---

## Verify S3 Upload

```bash
aws s3 ls s3://maab-customer-data-processing/
```

---

## Generate CPU Load for CloudWatch Alarm Testing

```bash
yes > /dev/null &
yes > /dev/null &
yes > /dev/null &
```

---

## Stop CPU Stress Test

```bash
pkill yes
```

---

## Verify CloudTrail Logs

```bash
aws cloudtrail describe-trails
```

---

## Verify Existing AWS Resources

### List EC2 Instances

```bash
aws ec2 describe-instances
```

### List S3 Buckets

```bash
aws s3 ls
```

### List RDS Databases

```bash
aws rds describe-db-instances
```
