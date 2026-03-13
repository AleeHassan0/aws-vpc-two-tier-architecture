SSH Commands

Connect to Bastion Host

ssh -i frankfurt.pem ec2-user@bastion-public-ip

Copy key to Bastion Host

scp -i frankfurt.pem frankfurt.pem ec2-user@18.185.105.151:/home/ec2-user

Secure key

chmod 400 frankfurt.pem

Connect to Private Instance

ssh -i frankfurt.pem ec2-user@private-ip
