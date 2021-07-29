# Username and Password

You can get the credentials of Database and OS from this chapter.

## Database

### Database Password

#### Linux

For Linux, the database password is stored in the file of your instance: *`/credentials/password.txt`* 

Connect to the instance by using SSH and run the command `sudo cat /credentials/password.txt` to get username and passwords.

![Run cat command](https://libs.websoft9.com/Websoft9/DocsPicture/zh/common/catdbpassword-websoft9.png)

#### Windows

For Windows, the database password is stored in the file of your instance: 
 *`c:/credentials/password.txt`*

You can also find the shortcut for password file from the Windows Desktop.

### Database Username and GUI

Different databases have certain differences. Refer to the following table：

| Database                    | Username     | GUI           |
| ----------------------- | ---------- | ------------------------ |
| MySQL/Mariadb with PHP | root       | http://Internet IP/phpmyadmin |
| MySQL/Mariadb     | root       | http://Internet IP:9090       |
| PostgreSQL              | postgres   | http://Internet IP:9090       |
| Mongodb                 | adminmongo | http://Internet IP:9091       |
| Oracle                  | system     | NO                     |
| SQLServer               | sa         | SQLServer Management Studio,one Desktop client     |



## OS

When creating AWS EC2, it only supports key pair for verification.

![Key pair](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2createpw-websoft9.png)

Additionally, there is different username for different OS and different distributions.

### Linux

- For Amazon Linux 2 or Amazon Linux AMI, the username: ec2-user.
- For a CentOS AMI, the username: centos.
- For a Debian AMI, the username: admin or root.
- For a Fedora AMI, the username: ec2-user or fedora.
- For a RHEL AMI, the username: ec2-user or root.
- For a SUSE AMI, the username: ec2-user or root,
- For an Ubuntu AMI, the username: ubuntu.

Otherwise, if ec2-user and root don't work, check with the AMI provider.

The above information comes from AWS Official, view [more](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/connection-prereqs.html).

### Windows

The username is  `Administrator`.