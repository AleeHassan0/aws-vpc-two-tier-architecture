Route Tables

Public Route Table

Name: RT for public

Routes:

192.168.0.0/24 → local  
0.0.0.0/0 → Internet Gateway

This route table is attached to:

- public-subnet-1
- public-subnet-2

Private instances use the main route table.

Traffic flow:

Private EC2 → NAT Gateway → Internet Gateway
