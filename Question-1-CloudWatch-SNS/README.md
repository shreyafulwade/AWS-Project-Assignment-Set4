# Project 1 – AWS CloudWatch Monitoring with SNS

## Objective

The objective of this project is to configure Amazon CloudWatch monitoring for an EC2 instance, monitor CPU utilization and instance health, create a CloudWatch alarm for high CPU usage, and configure Amazon SNS to send an email notification when the alarm is triggered.

## AWS Services Used

- Amazon EC2
- Amazon CloudWatch
- Amazon SNS

## Architecture

EC2 Instance
        ↓
Amazon CloudWatch
        ↓
CloudWatch Alarm
        ↓
Amazon SNS
        ↓
Email Notification

## Implementation Steps

### 1. EC2 Instance

An Amazon EC2 instance was created and its instance status was checked successfully.

### 2. Instance Health Monitoring

The EC2 instance health and status were monitored using Amazon CloudWatch.

### 3. CPU Utilization Monitoring

CloudWatch was configured to monitor the CPU utilization of the EC2 instance.

### 4. CloudWatch Alarm

A CloudWatch alarm was created to monitor high CPU utilization.

### 5. Amazon SNS Configuration

An Amazon SNS topic was created and an email subscription was configured for receiving alarm notifications.

### 6. Testing

The CloudWatch alarm and SNS notification configuration were tested successfully.

## Screenshots

The following screenshots demonstrate the implementation:

1. EC2 Instance
2. EC2 Instance Status and Health Check
3. CloudWatch CPU Utilization
4. CloudWatch Alarm Configuration
5. SNS Topic
6. SNS Email Subscription
7. CloudWatch Alarm State

## Result

The EC2 instance was successfully monitored using Amazon CloudWatch. CPU utilization and instance health were monitored, a CloudWatch alarm was configured for high CPU usage, and Amazon SNS was configured for email notifications.

## Conclusion

This project demonstrates how Amazon CloudWatch and Amazon SNS can be integrated with an EC2 instance for monitoring and automated email notifications.
