# Project: Custom VPC with Public & Private Subnets

## Overview
This project demonstrates the design of a secure AWS VPC architecture with network isolation.

The goal was to understand:
- Public vs private subnets
- Route table behavior
- Internet Gateway usage
- Why private resources should not be exposed

## Architecture Summary
- Custom VPC
- Public subnet with IGW route
- Private subnet with no internet route
- EC2 in private subnet
- Session Manager access via VPC endpoints

## Key Learning Points
- Subnet security is enforced by routing, not names
- Private EC2 can be managed without SSH
- VPC endpoints allow AWS service access without internet
- IAM + networking must work together

## Why This Matters
This architecture mirrors real production environments where application servers are isolated and accessed only through controlled paths.

## Lessons Learned
- Misconfigured routing breaks connectivity immediately
- IAM permissions alone are not enough without network access
- Security should be built into architecture, not added later
