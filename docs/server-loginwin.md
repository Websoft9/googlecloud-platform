# Windows Connect

As AWS requires [key pair](/server-create.md) to launch an instance, you need to get password before using Remote Desktop to connect to Windows server.

## Access Password

1. Login to AWS console, choose the instance which you want to connect to, click 【Connect】 and then click 【Get Password】 in the pop-up window.
   ![aws get password](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-winconnect-websoft9.png)

2. Upload the key pair stored locally.
   ![aws upload key pairs](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-winconnectpw-websoft9.png)

3. Click 【Decrypt Password】, then the password will be displayed on the interface.
   ![aws Decrypt Password](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-winconnectgpw-websoft9.png)

## Remote Connection

1. Choose a way to open a local computer remote desktop (three-in-one):

- - Open 【Start】>【Remote Desktop】.
  - Open 【Start】, input "mstsc" directly. The system will search for the Remote Desktop
  - Use the keyboard **Windows Logo** + **R** to start the command windows, and input input "mstsc" to open the Remote Desktop

2. Enter the public IP address of the instance in the Remote Desktop Connection dialog box, then click 【Show Options】.

   ![img](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/windows-remote.png)

3. Enter the username and check 【Allow me to save credentials】. In this way, you do not need to manually enter the password again when you log on later.
   ![img](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/windows-remote-login.png)

4.  Click 【Connect】 to complete connection to the instance.
   ![image.png](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/azure-windows2019desktop-websoft9.png)

5. After logging in remotely, you can 【copy】 the file directly from the local and 【paste】 the file to the server.
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/azure/azure-copyfilewin-websoft9.png)

6. If you want to use FTP, you need to install the FTP software by your yourself. (Recommended to use FileZilla Server)