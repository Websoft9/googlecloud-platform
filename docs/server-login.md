# Linux Connect

There are two ways to connect to a Linux server: command line and SFTP.

## Connect by Command

Command is the basic operation of the Linux system. AWS supports three ways to connect by Command:

| Tool                                                  | Instructions                                                     |
| ------------------------------------------------------ | ------------------------------------------------------------ |
| A standalone SSH client                                  | Download [putty](https://putty.org/) and other SSH clients to local computer to connect to Linux. |
| Hosting SSH client based on my browser (Alpha)               | Connect from AWS console website, the prerequisite is to install [EC2 Instance Connect](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-connect-set-up.html) on your instance. |
| A Java SSH client directly connected from my browser（Java required） | Directly connect from AWS console website, the prerequisite is to **install Java plugin**. |


Taking **Hosting SSH client based on my browser** as an example, steps for how to connect to a Linux server are as follows:

1. Refer to [Set up EC2 Instance Connect](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-instance-connect-set-up.html) to install EC2 Instance Connect module（For Websoft9 image, the module is installed by default, just skip this step.）

2. Login to AWS EC2 console, open 【Instance】> 【Connect】and choose the second way to connect.
   ![command line](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-connectmethods-websoft9.png)

3. Click 【Connect】, a window opens and you are connected to the instance.

After you're connected to the server through command line, the following two most common examples of operations are required.

### Sample 1: Get database password  



For security reasons, each time a user deploys, a unique random database password is generated and stored in the service. Just require the following command to view:

```shell
sudo cat /credentials/password.txt

//result
MySQL username:root
MySQL Password:@qDg1Vq1!V
```

### Sample2: Enable the root username  


For security and regulatory requirements, AWS does not open the Linux root account by default, and only provides users with a common account. If you wish to use the root account, enable it by following the steps below:

```shell
sudo su
sudo sed -i 's/#PermitRootLogin yes/PermitRootLogin yes/' /etc/ssh/sshd_config
sudo systemctl restart sshd
sudo passwd root
```

## Connect by SFTP

SFTP is an FTP mode that uses the SSH protocol, also known as security-enhanced FTP. The SFTP tool is a favorite operation mode for Linux users. The following is an example of WinSCP SFTP tool to detail the use of SFTP.

### Configure WinSCP

1. Download [WinSCP](https://winscp.net/eng/docs/start) and install it, then start it and create a new connection.

2. Two verifications of cloud server: **password verification and key-key pair verification**

   - Password authentication（the most common way）
     ![password authentication](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/winscp-newsite.png)

   - Key-key pair authentication
     ![key-key pair authentication](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/winscp-secrets-websoft9.png)

3. You may want to save your session details to a site so you do not need to type them in every time you want to connect. Press 【Yes】 button and type site name. 
   ![Save session](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/winscp-sessionsave-websoft9.png)

4. You can see this interface if the connection is valid.
   ![WinSCP GUI](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/websoft9-winscp-success.png)

### Manage files

For WinSCP, you can easily upload and download files by dragging and dropping, and can perform various settings and operations on files (folders).


1. In general, the files on the website are placed in the */data/wwwroot* directory.
   ![upload files](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/winscp-dragfile-websoft9.png)

2. You can perform multiple operations on the VM by right-clicking on a file or folder on the server.
   ![set file](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/websoft9-winscp-youjian.png)

3. The relevant interface for modifying file permissions is as follows:

   ![group and owner setting](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/websoft9-winscp-quanxian.png)

### Run command

WinSCP has a built-in command run function. Although the command function is limited to running non-interactive naming (that is, no feedback and process input are required during command execution), it is simple and practical for beginners.

1. WinSCP logs in to the server, then click on the command window icon from the menu (shortcut Ctrl+T is also available) 
   ![command of WinSCP](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/winscp-ucmd-websoft9.png)

2. Execute the command (one command at a time) in the pop-up command run window. Eg: To query the memory usage, run the command `free -m`
   ![command of WinSCP](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/wincp-showmemory-websoft9.png)

### Integrate Putty

Under certain specificities, you may need to use [Putty](https://putty.org/) to run commands. Since Putty is a command operation interface, you need to enter the root password every time you use it. If the password is complicated, it will make people feel troublesome. In fact, WinSCP can be integrated with Putty. After integration, you can open Putty through WinSCP and log in to the server automatically.

1. Open the 【Preferences】>【Integration】>【Application】 and input the local address of your Putty, click OK.
   ![Putty Address](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/websoft9-winscp-putty.png)

2. After completing the integration, you only need to open the Putty through Winscp's window shortcut. 
   ![open window on WinSCP](http://libs.websoft9.com/Websoft9/DocsPicture/en/winscp/websoft9-winscp-puttyopen.png)

> Opening a Putty operation via Winscp is no different than opening a putty directly.