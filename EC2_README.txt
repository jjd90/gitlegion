Create an EC2 Instance in AWS:

1.	Navigate to the AWS Instances and click “Launch Instance.”
•	Select your desired operating system
•	Chose an instance type. This will very depending on the magnitude of expected traffic.
•	Configure the server details, add storage, add tags,  and configure the security groups.
•	When all the specifications are created click “Review and Launch.”
•	Make sure to save your private key, you won’t be able to go back.
2.	SSH into your EC2 instance
•	Follow the instructions under the “connect” tab
•	Windows users will need to download Putty-Gen to convert the private key into a public key (ssh-keygen is the linux command)
3.	Give Users SSH Public Keys
•	Create a user
•	Sudo su – username
•	In the home directory create the directory and file .ssh and .ssh/authorized_keys respectively. 
•	Chmod 700 .ssh
•	Chmod 600 authorized_keys
•	Add the public key into the authorized_keys file
