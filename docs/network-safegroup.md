# Safe Group

A security group is a function of managing the EC2 port, which is a channel for access application from external access. Let's take **opening port 80** as an example to introduce you to the use of security groups.

1. Login to AWS console and open 【EC2】>【Instances】.  

2. Open 【Description】and then click the name of Security groups.
   ![ec2 edit security group](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-changesg-websoft9.png)
3. Enter the setting interface, click 【Inbound】and 【Edit】.
   ![ec2 edit](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-sfin-websoft9.png)
4. Edit inbound rule and add a new one.
   ![ec2 edit rule](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-set80sg-websoft9.png)
3. Save it.