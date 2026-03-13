EC2 Instances

2 Bastion Hosts
for redundancy

Subnet: public-subnet-1 & public-subnet-2  
Purpose: secure SSH access to private instances.

Database EC2

Subnet: private-subnet-1  
Purpose: run MySQL database.

Another database instance exists in private-subnet-2 for redundancy.
