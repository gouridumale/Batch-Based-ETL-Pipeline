# Batch Based ETL Pipeline

# Overview

This project demonstrates a batch-based ETL (Extract, Transform, Load) pipeline using AWS services. The pipeline reads data from an S3 bucket, performs data integrity checks and transformations using AWS Glue, and loads the transformed data into an RDS instance.

# The architecture includes:

AWS Lambda: For initial processing and triggering the Glue job.

AWS Glue: For data transformation.

Amazon S3: For storing source and processed data.

Amazon RDS: For storing the final transformed data.

Amazon DynamoDB: For auditing and logging.
image

# Project Structure

Batch Based ETL Pipeline Documentation.pdf: Detailed documentation of the project.
Scripts/

Glue Script/ETL_Job_to_RDS.py: Glue job script for data transformation and loading.

fake_Data_generator_Script/fake_data_script.py: Script for generating fake data.

lambda_function script/lambda_function (1).py: Lambda function script for initial processing and triggering Glue job.
Setup Instructions


IAM Roles: Create necessary IAM roles with appropriate permissions.

S3 Buckets: Create source and processed data buckets in S3.

RDS Instance: Set up an RDS instance and ensure it is accessible.

DynamoDB Table: Create a DynamoDB table for auditing.

AWS Glue Job: Set up the Glue job with the provided script.

Lambda Function: Deploy the Lambda function with the provided script.
Running the Pipeline

Upload Data: Upload the data to the source S3 bucket.
Trigger Lambda: Trigger the Lambda function manually or through a CloudWatch event.
Monitor Glue Job: Monitor the Glue job for successful completion.
Query RDS: Verify the transformed data in the RDS instance.
Conclusion

This project provides a comprehensive example of setting up and running a batch-based ETL pipeline using AWS services. It demonstrates the integration of various AWS components to achieve a seamless data processing workflow.
