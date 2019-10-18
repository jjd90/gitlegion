
~Route 53 Domain Setup~

1. Purchase Top Level Domain (I used Google Domains)
2. Sign into AWS, go to Route 53
3. Create hosted zone using the domain that was purchased
4. 4 Name Server Records will be created as well as a Start Of Authority Record.
5. Return to Google Domains and copy the NS records to custom host
5. Copy the IP Address from the EC2 Instance within AWS and use it to create a Type A Record Set. 
6. Create Alias record for www

For the Certification step I was given the CNAME Record Information by Yousef
