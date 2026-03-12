Subnet Design

The VPC is divided into four subnets.

Public Subnet 1
CIDR: 192.168.0.0/26
Availability Zone: eu-central-1a

Public Subnet 2
CIDR: 192.168.0.64/26
Availability Zone: eu-central-1b

Private Subnet 1
CIDR: 192.168.0.128/26
Availability Zone: eu-central-1a

Private Subnet 2
CIDR: 192.168.0.192/26
Availability Zone: eu-central-1b

Public subnets host web servers or  bastion hosts.

Private subnets host database servers.
