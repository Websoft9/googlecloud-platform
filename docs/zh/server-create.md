# 创建

下面介绍 AWS 上服务器实例的创建方式（ AWS 称之为**启动实例**）。

创建实例最基本的条件是需要给服务器准备一个系统盘的启动模板文件，这个模板最常见的表现形式就是镜像文件

下面介绍基于镜像创建云服务器的操作步骤：

## 创建EC2

1. 登录到AWS管理控制台，点击“EC2”，
   ![进入ec2控制台](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-ec2-websoft9.png)

2. 进入EC2控制面板，点击“启动实例”，即开始创建一个新的实例
   ![启动实例](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-addec2-websoft9.png)

3. 在映像一栏，点击“浏览所有公用和专用映像”，然后搜索关键件词“websoft9”，列出相关镜像
   ![选择Websoft9镜像](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-ec2image-websoft9.png)

4. 选择一个你所需的镜像（以Odoo为例），开始创建EC2实例 

5. 后续动作基本都会要求用户完成：选择实例类型、VPC、Key Pair等设置
   ![选择Websoft9镜像](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-ec2createpw-websoft9.png)

6. 等待几分钟，EC2创建完成后，镜像会作为EC2实例的系统盘启动，即镜像自动部署到实例中

## 秘钥对

在创建EC2时，AWS要求使用秘钥对登录，下面是创建秘钥对步骤

1. 登录AWS控制台，打开：EC2 Dashboard->网络与安全->秘钥对，点击“**创建秘钥对**”按钮
   ![创建秘钥对](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-createkeyps-websoft9.png)

2. 为秘钥对命名，例如“myKey”
   ![秘钥对名称](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-keypsname-websoft9.png)
   
3. 将秘钥对文件 myKey.pem 保存到本地电脑