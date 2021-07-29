# 连接Windows

AWS 只支持[秘钥对](/zh/server-create.md#秘钥对)创建实例，因此在远程连接 Windows 服务器之前需要上传秘钥对获取密码

## 获取密码

1. 登录AWS控制台，找到需要登录的服务器，点击“连接”在弹出的窗口中点击【Get Password】
   ![AWS Get Password](http://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-winconnect-websoft9.png)

2. 上传创建服务器的时候保存的**私钥**
   ![AWS upload key pair](http://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-winconnectpw-websoft9.png)

3. 点击【Decrypt Password】之后，密码解锁成功，并显示在界面上
   ![AWS Descypt Password](http://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-winconnectgpw-websoft9.png)

## 远程桌面连接

1. 选择一种打开本地电脑远程桌面的方式（三选一）: 
   - 打开 **开始菜单** -> **远程桌面连接**
   - 打开 **开始菜单**，输入”mstsc“ ，系统会搜索远程桌面连接工具
   - 通过 **Windows Logo** + **R** 打开系统的命令窗口，输入”mstsc“来启动远程桌面连接工具

2. 打开远程桌面连接，输入公网IP地址
   ![img](http://libs.websoft9.com/Websoft9/DocsPicture/zh/windows/windows-remote.png)

3. 通过更多选项，设置默认用户名，例如”Administrator“，并勾选”允许我保存凭据“
   ![img](http://libs.websoft9.com/Websoft9/DocsPicture/zh/windows/windows-remote-login.png)

4. 点击连接，成功后会看到Windows界面
   ![image.png](http://libs.websoft9.com/Websoft9/DocsPicture/en/azure/azure-windows2019desktop-websoft9.png)

5. 远程登录后，就可以直接从本地**拷贝**文件，然后**粘贴**文件到服务器上。
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/azure/azure-copyfilewin-websoft9.png)

6. 如果需要使用FTP，需要自行在云服务器上安装 FTP 软件（推荐使用FileZilla Server）