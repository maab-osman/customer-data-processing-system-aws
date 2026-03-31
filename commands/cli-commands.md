# Create table
CREATE TABLE customers (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100)
);

# Insert data
INSERT INTO customers (name, email)
VALUES ('Alice', 'alice@email.com'),
       ('Bob', 'bob@email.com');

# Query
SELECT * FROM customers;

# Upload to S3
aws s3 cp customer.csv s3://<bucket-name>/

# List S3
aws s3 ls s3://<bucket-name>/
