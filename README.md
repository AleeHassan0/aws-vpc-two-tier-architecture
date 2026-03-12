 AWS VPC Two-Tier Architecture

This project demonstrates how to design a secure AWS infrastructure using a custom VPC with public and private subnets.

The architecture separates web servers from database servers to improve security.


 Key Components

- Custom VPC
- Public Subnets
- Private Subnets
- Internet Gateway
- NAT Gateway
- Bastion Host
- Web Servers
- Database Servers

 Architecture Design

Public Layer:
- Web Servers
- Bastion Host

Private Layer:
- Database Servers

Database instances cannot be accessed directly from the internet.

Access flow:

Laptop → Bastion Host → Private Database EC2

 Networking

VPC CIDR: 192.168.0.0/24

Public Subnets:
- 192.168.0.0/26
- 192.168.0.64/26

Private Subnets:
- 192.168.0.128/26
- 192.168.0.192/26

 Security Design

- SSH restricted to Bastion Host
- Database instances in private subnets
- NAT Gateway for outbound internet access
- Internet Gateway only for public subnets

Learning Outcomes

- Designing AWS VPC networks
- Subnetting and CIDR planning
- Route table configuration
- Internet Gateway vs NAT Gateway
- Secure Bastion Host access
- Managing private infrastructure
