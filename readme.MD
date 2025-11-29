# Terraform AWS VPC

This module creates the following resources.
* VPC
* IGW
* 2 Public subnets in uas-east-1a and us-east-1b AZ
* 2 Private subnets in uas-east-1a and us-east-1b AZ
* 2 Database subnets in uas-east-1a and us-east-1b AZ
* 1 Public Route table
* 1 Private Route table
* 1 Database Route table
* 1 EIP for NAT
* NAT Gatewau in public subnet 1a az
* IGW route is added to public route table
* NAT gateway route to private and database route tables
* Route table associtation with subnets
* VPC to default VPC peering
* Public route table to default VPC route
* Default VPC main route table to created VPC route

### Inputs

* vpc_cidr - (Required). User must supply the CIDR for VPC
* project_name - (Required). User must supply the Porject name
* environment - (Required). User must supply the environment