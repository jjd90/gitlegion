# How to create a VPC in AWS:

1. Configure the region to US West - Oregon
2. Create the base VPC using the setup wizard
- make sure to check the "VPC with Public and Private Subnets" option
- make sure to keep most of the default values, except:
  a. select an availability zone under the public subnet value (us-west-2b)
  b. select the same availability zone under the private subnet value
3. Click "Create VPC"
4. Connect this VPC to the EC2
5. Create 2 more public and 2 more private subnets
- on the Services menu, click "VPC"
- click "Subnets", then "Create Subnet"
- Set the following values: Name tag, Availability Zone (different from the one used), VPC, CIDR Block
- Click "Yes Create"
6. Do this for the rest of the private/public subnets
7. Separate public and private subnets in two different routing tables
8. Create the Internet Gateway
