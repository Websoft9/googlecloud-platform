# Launch

The introduction below is about how to launch instance on AWS.

The basic condition for launching instance is to prepare a boot disk file for the system disk for the instance. The most common template file is image.

Steps below are about how to launch instance based on image:

## Create EC2

1. Login to AWS Management Console, and click 【EC2】.
   ![log in](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2-websoft9.png)

2. Enter EC2 Dashboard, and click 【Launch Instance】to create Instance.
   ![launch instance](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-addec2-websoft9.png)

3. When choosing AMIs, click 【View all public and private AMIs】 and search keyword "websoft9" to see the list of images.
   ![choose image of Websoft9](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2image-websoft9.png)

4. Select the image you need.

5. Finish the following steps, which require you to choose instance type, VPC, set key pair and more.
   ![create instance](http://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2createpw-websoft9.png)

6. Wait several minutes after completing creating EC2, and the image is started as the system disk of the instance, that is, the image is automatically deployed to the instance.

## Key Pair

When launching instance, AWS requires key pair to log in. Steps for how to create key Pair are as follows:

1. Login to AWS console, open 【EC2 Dashboard】>【NETWORK & SECURITY】>【Key Pairs】and click 【Create Key Pair】.
   ![create key pair](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-createkeyps-websoft9.png)

2. Name the key pair, such as "myKey".
   ![name](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-keypsname-websoft9.png)
   
3. Store key pair file **myKey.pem** into the local computer.