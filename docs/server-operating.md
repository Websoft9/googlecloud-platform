# Manage

Some common operations to EC2 are as follows:

## Start, Stop and Terminate

You can change the instance state on EC2 console, including:

- Start
- Stop
- Reboot
- Terminate
- Recover

![aws EC2 state Websoft9](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2state-websoft9.png)

> Terminate=Delete EC2

If you want to automatically recover the instance when it becomes impaired due to an underlying hardware failure or a problem that requires AWS involvement to repair, you need to enable [CloudWatch alarms](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-recover.html) previously.

## Instance settings

Follow the steps below to change instance type：

1. Login to AWS console and stop the instance.

2. Open 【Actions】>【Instance Settings】>【Change Instance Type】.
   ![adjust configuration](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-configures-websoft9.png)

3. Complete new settings, then start the instance.

## Get system log

You can get system log on EC2 console：

1. Login to AWS console and stop the instance.

2. Open 【Actions】>【Instance Settings】>【Get System Log】.
   ![get system log](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-getsyslogs-websoft9.png)
3. Complete the new settings, then start the instance.
   ![display system log](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-syslogs-websoft9.png)