# Private EC2 Managed via AWS Systems Manager

## Goal
Design a secure EC2 instance that is not exposed to the internet but remains fully manageable.

## Architecture
- EC2 instance in a private subnet
- No public IP
- No inbound security group rules
- IAM role: AmazonSSMManagedInstanceCore
- VPC interface endpoints for SSM services

## Key Concept
Private resources cannot access AWS APIs without a network path.
VPC endpoints provide private connectivity to Systems Manager without using the internet.

## Result
The instance is fully manageable through Session Manager while remaining isolated from public access.

This mirrors production security architecture used in enterprise environments.
