# Deploy Images

[Websoft9](https://www.websoft9.com) has published hundreds of images (referred to as **AMIs**) on AWS Marketplace, which cover most common application scenarios and have received good feedback from users.

> Want to deploy image of Websoft9? Click [here](https://aws.amazon.com/marketplace/seller-profile?id=c639a579-182c-4d30-8578-4d4d89fba658) to choose from all great images of Websoft9 on AWS Marketplace.

How to deploy image? There are two methods:

## Deployment by Marketplace

1. Log in [AWS Marketplace](https://aws.amazon.com/marketplace).

2. Search "Websoft9" and view the list of images of Websoft9.
   ![Search image of Websoft9](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-mkss-websoft9.png)  

3. Click the image you want, then click 【Continue to Subscribe】 after jump to the product page.
   ![Subscribe image](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-rs-websoft9.png)

4. Accept Terms and Conditions as the system prompts.

5. After the system prompts you've finished the subscribing, click the button 【Continue to Configuration】 for preparation before creating EC2.
   ![Configuration](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-cc-websoft9.png)

5. Check the information required, then click 【Continue to Launch】 to start launching.
   ![Continue to Launch](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-imagecreate-websoft9.png)

6. Choose from three actions in the process of creating EC2.
   ![Start to Launch](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-imagecreate2-websoft9.png)

   - Launch through EC2 （the recommended way ）
   - Launch from Website
   - Copy to Service Catalog

7. Complete the following steps, including choosing an instance type, setting VPC, Key Pair and so on.

8. Wait several minutes after completing creating EC2, and the image is started as the system disk of the instance, that is, the image is automatically deployed to the instance.


## Deployment by EC2

1. Login to the AWS Management Console, and click 【EC2】.
   ![Log in console](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2-websoft9.png)

2. Enter EC2 Dashboard, and click 【Launch Instance】to create Instance.
   ![Launch Instance](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-addec2-websoft9.png)

3. When choosing AMIs, click 【View all public and private AMIs】 and search keyword "websoft9" to see the list of images.
   ![Choose image of Websoft9](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2image-websoft9.png)

4. Select the image you need and click【Continue】to subscribe.
   ![Continue to subscribe](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-createdec2-imageselected-websoft9.png)

5. Finish the following steps, which require you to choose instance type, add storage, configure security group, set key pair and more.
   ![Create Instance](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-createdec2-chooseinstances-websoft9.png)

6. Wait several minutes after completing creating EC2, and the image is started as the system disk of the instance, that is, the image is automatically deployed to the instance.


> In addition to image deployment, you can git our Ansible Scripts on [Github](https://github.com/websoft9) for Ansible automation.