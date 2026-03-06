# AWS S3 → Lambda Event Trigger (CloudFormation)

This project demonstrates a simple event-driven AWS architecture built using Infrastructure as Code.

## Architecture

S3 → Lambda → CloudWatch Logs

When a file is uploaded to the S3 bucket, a Lambda function is automatically triggered and logs event metadata to CloudWatch.


## Project Structure

aws-s3-lambda-cloudformation
│
├── template for CloudFormation.yaml
├── README.md
│
├── screenshots
│   ├── cf-stack-overview.png
│   ├── cf-resources.png
│   ├── s3-upload.png
│   ├── cloudwatch-logs.png
│   ├── architecture-flow.png
│   └── visual-designer.png

## Services Used

- AWS CloudFormation
- Amazon S3
- AWS Lambda
- AWS IAM
- Amazon CloudWatch

## Architecture Diagram

User Upload → S3 Bucket → Lambda → CloudWatch Logs

## What the Lambda Function Logs

- Bucket name
- File name
- Event timestamp

## Deployment Steps

1. Open AWS CloudFormation
2. Create a new stack
3. Upload `template.yaml`
4. Wait for stack status **CREATE_COMPLETE**
5. Upload a file to the S3 bucket
6. Check Lambda logs in CloudWatch

## Learning Goals

- Infrastructure as Code
- Event-driven architectures
- AWS service integration
- IAM permissions
- Serverless workflows

## Screenshots

### 1. CloudFormation Stack Overview

![CloudFormation Stack](cf-stack-overview.png)

### 2. CloudFormation Resources

![CloudFormation Resources](cf-resources.png)

### 3. Uploading File to S3

![S3 Upload](s3-upload.png)

### 4. CloudWatch Logs (Lambda Execution)

![CloudWatch Logs](cloudwatch-logs.png)

### 5. Architecture Flow

![Architecture Flow](architecture-flow.png)

### 6. CloudFormation Visual Designer

![CloudFormation Visual Designer](visual-designer.png)
