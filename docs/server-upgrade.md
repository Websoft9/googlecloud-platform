# Upgrade

There are two options for updating the OS. One is launching **AWS Systems Manager** solution on AWS console, and the other is using the OS's upgrade solution.

## AWS Systems Manager

AWS offers [AWS Systems Manager](https://docs.aws.amazon.com/systems-manager/latest/userguide/) solution, which can help you automate collecting software inventory, patching applications OS, launching system VMs, and configuring Windows and Linux.

1. Login to AWS Management Console and open 【AWS System Manager】 service.

2. Open 【Instances & Nodes】>【Patch Manager】to enter the manage interface.
![launch system manager](http://libs-websoft9-com.oss-cn-qingdao.aliyuncs.com/Websoft9/DocsPicture/en/aws/aws-sysmupdate-websoft9.png)

3. Follow the guide to complete upgrading.

## Upgrade by OS

Upgrading by OS is implemented by logging in to the EC2, inputting an update command or an operation update function, which is different from the update management function of the AWS portal.

### Upgrade Linux 

To upgrade Linux OS, you only need to run an update command to install most updates.

```shell
#CentOS or Redhat
sudo yum update -y

#Ubuntu
apt update && apt upgrade -y
```

In fact, the image provided by Websoft9 has periodically executed the above update commands through cron of Linux.

### Upgrade Windows

The update of the Windows server is similar to that of the local computer. Just Manually find the update management program and set the automatic download and automatic update.