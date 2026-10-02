# Project 3 – Secure AWS VPC with Public and Private Subnets

## Objective

The objective of this project is to design and configure a secure AWS VPC containing both public and private subnets, deploy EC2 instances in each subnet, configure an Internet Gateway for the public subnet, and configure a NAT Gateway to provide internet access to the private subnet.

## AWS Services Used

- Amazon VPC
- Amazon EC2
- Internet Gateway
- NAT Gateway
- Route Tables
- Public Subnet
- Private Subnet

## Architecture

Internet
   |
Internet Gateway
   |
Public Subnet
   |
Public EC2 Instance

Private Subnet
   |
Private EC2 Instance
   |
NAT Gateway
   |
Internet Gateway
   |
Internet

## Implementation Steps

### 1. Create VPC

An AWS VPC was created to provide an isolated network environment for the EC2 instances.

### 2. Create Public and Private Subnets

Two subnets were created:

- Public Subnet
- Private Subnet

### 3. Configure Internet Gateway

An Internet Gateway was attached to the VPC and configured for the public subnet.

### 4. Configure Route Tables

A public route table was configured with a route to the Internet Gateway.

A private route table was configured to route internet-bound traffic through the NAT Gateway.

### 5. Configure NAT Gateway

A NAT Gateway was created in the public subnet to provide outbound internet access to the private subnet.

### 6. Deploy EC2 Instances

One EC2 instance was deployed in the public subnet and another EC2 instance was deployed in the private subnet.

### 7. Test Connectivity and Security

The connectivity between the public and private resources was tested.

The public EC2 instance can communicate with the internet through the Internet Gateway, while the private EC2 instance can access the internet through the NAT Gateway without being directly accessible from the public internet.

## Screenshots

The following screenshots demonstrate the implementation:

1. VPC Configuration
2. Public Subnet
3. Private Subnet
4. Internet Gateway
5. Public Route Table
6. Private Route Table
7. NAT Gateway
8. Public EC2 Instance
9. Private EC2 Instance
10. Connectivity Testing

## Result

The VPC was successfully configured with public and private subnets. The public EC2 instance was connected through the Internet Gateway, while the private EC2 instance received outbound internet access through the NAT Gateway.

## Conclusion

This project demonstrates how AWS VPC networking can be designed using public and private subnets, Internet Gateway, NAT Gateway, route tables, and EC2 instances to provide controlled and secure network connectivity.
