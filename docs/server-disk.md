# Volumes (Disk)

For AWS, volume can be a separate computing resource (created separately, billed separately, managed separately, etc.) and can be integrated into an instance as a component.

## Create Volume

1. Login to AWS console and open EC2 Dashboard.

2. Open 【ELASTIC BLOCK STORE】>【Volumes】 to create volume.
   ![create volume](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-createvolume-websoft9.png)
   
3. Complete volume type, size and other settings, then check before creating.
   ![volume settings](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-createvolume2-websoft9.png)
   
4. Attach the volume created to the instance.
   ![attach volume](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-volumeaddec2-1-websoft9.png)
   
   ![attach volume](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-volumeaddec2-2-websoft9.png)
   
5. Log in to the instance, and complete volume initialization to make it available.
    - For Windows, view official document [Making an Amazon EBS volume available for use on Windows](https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/ebs-using-volumes.html)
    - For Linux, view official document [Making an Amazon EBS volume available for use on Linux](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ebs-using-volumes.html) 

6. Complete all settings and the volume is available.

## Detach Volume

To detach volume from the instance, refer to the steps below:

1. Login to AWS console and open EC2 Dashboard.  

2. Open 【Instances】, choose the instance from which the volume will be detached and click 【Stop】.  

3. Open【ELASTIC BLOCK STORE】>【Volumes】, choose the volume and click 【Detach Volume】.
   ![detach volume](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-detachvolume-websoft9.png)

> The volume detached remains in the storage account and wouldn't be deleted.



## Modify Volume

If the volume is not attached to instance, it can be modified.

1. Login to AWS console and open 【EC2->ELASTIC BLOCK STORE】>【Volumes】.  

2. Choose the volume need to modify and open 【Actions】>【Modify Volume】.
   ![modify volume](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ddiskin-websoft9.png)  

3. Set new size.

> In most cases, the volume can only increase in size, but can not decrease.