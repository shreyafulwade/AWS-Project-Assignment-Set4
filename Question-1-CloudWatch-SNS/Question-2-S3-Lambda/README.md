# Project 2 – AWS S3 and Lambda Event-Driven Solution

## Objective

The objective of this project is to create an Amazon S3 bucket, configure an AWS Lambda function, connect S3 with Lambda, and process an event when a file is uploaded to the S3 bucket.

## AWS Services Used

- Amazon S3
- AWS Lambda
- Amazon CloudWatch Logs

## Architecture

S3 Bucket
    ↓
File Upload Event
    ↓
AWS Lambda
    ↓
CloudWatch Logs

## Implementation Steps

### 1. Create S3 Bucket

An Amazon S3 bucket was created to store files and objects.

### 2. Upload File to S3

A file was uploaded to the S3 bucket to generate an S3 event.

### 3. Create Lambda Function

An AWS Lambda function was created using Python to process the S3 event.

### 4. Configure Lambda Code

Python code was deployed in the Lambda function to receive the S3 event and process the bucket and object information.

### 5. Connect S3 with Lambda

An S3 event notification was configured to trigger the Lambda function whenever a file was uploaded to the bucket.

### 6. CloudWatch Logs

The Lambda function execution was monitored using Amazon CloudWatch Logs.

The logs were checked to verify that the S3 bucket and uploaded object information was received successfully.

## Screenshots

The following screenshots demonstrate the implementation:

1. S3 Bucket Created
2. File Uploaded to S3
3. Lambda Function Created
4. Lambda Python Code
5. S3 and Lambda Connection
6. CloudWatch Logs

## Result

The S3 bucket was successfully connected with the Lambda function. When a file was uploaded to the S3 bucket, the Lambda function was triggered and the event details were successfully recorded in CloudWatch Logs.

## Conclusion

This project demonstrates an event-driven architecture using Amazon S3 and AWS Lambda, with CloudWatch Logs used to monitor Lambda execution.
