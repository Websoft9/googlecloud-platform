# Troubleshooting

Below are the most common problems caused by failures or setup errors.

If you have made it clear that the problem is caused by EC2, please view [Troubleshooting EC2 instance](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-troubleshoot.html).

#### Can't connect SFTP?

Check that the account number and password are correct. Please ensure that port 22 of [Server security group](/network-safegroup.md) is enabled.

#### Windows Remote Desktop Connection failed?

Check that the account number and password are correct. Please ensure that port 3389 of [Server security group](/network-safegroup.md) is enabled.

#### Can't restart the instance?

Please contact AWS Official for repair.

#### Http://public IP can not open the software initialization interface?

Check if the required software is installed, please ensure that port 80 of [Server Security Group](/network-safegroup.md) is enabled.