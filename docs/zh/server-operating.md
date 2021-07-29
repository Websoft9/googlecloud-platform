# 操作

下面是一些常见的EC2操作

## 启动、停止和终止

在EC2控制台可以对实例状态进行修改，包括：

- 启动
- 停止
- 重启
- 终止
- 自动恢复

![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-ec2state-websoft9.png)

> 终止=删除EC2

自动恢复的前提，必须启用[CloudWatch功能](https://docs.aws.amazon.com/zh_cn/AWSEC2/latest/UserGuide/ec2-instance-recover.html)，在实例受损（由于发生基础硬件故障或需要 AWS 参与才能修复的问题）时自动恢复实例。

## 调整配置

EC2的配置可以随时调整，具体操作如下：

1. 登录到AWS控制台，停止实例
2. 依次打开：操作->实例设置->更改实例类型
   ![调整配置](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-configures-websoft9.png)
3. 选择一个新的配置，启动实例

## 获取日志

EC2控制台可以方便的获取系统日志：

1. 登录到AWS控制台，停止实例
2. 依次打开：操作->实例设置->获取系统日志
   ![获取系统日志](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-getsyslogs-websoft9.png)
3. 选择一个新的配置，启动实例
   ![显示系统日志](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-syslogs-websoft9.png)