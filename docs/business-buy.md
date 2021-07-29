# Subscriptions

Below is the simple guide for subscriptions on AWS Marketplace:

## About

Subscription means buying. When you have completed [image deployment](/stack-deployment.md) on AWS, that means you have a subscription for this image.  

On AWS, costs of image is charged hourly or annually.

* Users may choose charging ways at will.
* Once the image is used on instance, the image Usage Quantity= Instance Usage Quantity
* If want to cancel the image subscription, you need to delete the corresponding instance.
* The instance stops running while the image remains charging.
* Annual subscription can be canceled.

## Choose version

There are several versions for each software. The default version is tha latest one, and you can change it by following the steps below:

1. When choose image, click【Previous version】.
   ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-subs-odoo-websoft9.png)

2. Drop down【Software version】and choose the version you want.
  ![](https://libs.websoft9.com/Websoft9/DocsPicture/zh/aws/aws-subs-odoooldversion-websoft9.png)


## Fee

There are free image and paid image on AWS Marketplace.

Websoft9 provides paid image on the AWS platform, and our profit model is to provide enterprise-level open source image and technical support services to customers who are willing to pay.

> If you want to use our product for free, please refer to our [Github project](https://github.com/websoft9)

Our image cost will be flexibly priced based on the number of instance CPU cores. The larger the number of cores, the higher the price generally.

Take the Odoo product we released as an example. The Software Cost listed by the Pricing on the product page is the image pricing.

![Websoft9 pricing](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-mkpricing-websoft9.png)

There are two billing way: Hourly (pay-per-Use) and Annual (pay yearly).

Terms are as follows：

``` text
Pay-per-Use: For pay-per-use images, you do not need to make payments when purchasing them. The system generates bills every hour based on the actual usage and deducts fees from your account balance.

Yearly: Yearly images are charged a one-time payment and take effect immediately upon purchase. You do not have the option to specify the start date of the images.

```

## View and Cancel

1. Login to AWS console.

2. Click the users name and choose 【Your Marketplace Software】 in the drop-down menu.
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-yoursb-websoft9.png)

3. View and cancel subscriptions.

## EULA

EULA (End User Licence Agreement) is a contract between one or more parties based on the proprietary rights of a licensor to grant a right to the licensee to use or access the subject matter of the licence.

Once you have deployment the image of Websoft9 on AWS, that means you have accept [*Websoft9 EULA*](https://support.websoft9.com/docs/legal/en/eula).
