# 备份

我们知道任何人（组织）都无法保证EC2永远正常运行状态。假如EC2出现无法启动或无法连接的故障，若没有备份会是什么样的后果？这样的教训是否值得尝试？

如果有备份，就能够恢复到备份之时的状态，大大降低损失。

AWS中对EC2实现备份的基本原理就是对EC2所属的磁盘做自动快照。

AWS控制台提供了两种备份入口：

## 快照备份

### 自动快照

1. 登录AWS控制台
2. 打开：EC2->ELASTIC BLOCK STORE->生命周期管理器，创建快照生命周期策略
    ![创建快照生命周期策略](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-snapshotauto-websoft9.png)
2. 根据提示完成快照策略设置

### 手动快照

如果不算自动备份，而是手动根据需要备份，步骤如下：

1. 登录到AWS控制台，打开EC2 Dashboard
2. 打开ELASTIC BLOCK STORE下的卷功能，选择一个卷后，实现“创建”快照操作
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-createsnapshot-websoft9.png)
3. 给快照命名后，开始创建

## AWS Backup

AWS中，AWS Backup 就是用于备份AWS设施的专项服务

1. 登录AWS控制台，打开：服务->存储->AWS Backup，创建一个备份计划 
   ![AWS Backup服务](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-backupservices-websoft9.png)
2. 在已有备份计划下，创建按需备份（即选择需要备份的云资源）
   ![AWS Backup服务](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-backupres-websoft9.png)
3. 资源类型为：EBS（磁盘），再选择一个列出的卷ID
   ![AWS Backup服务](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-backupres2-websoft9.png)
4. 完成其他备份设置