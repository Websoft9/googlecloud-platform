# FAQ

#### What Is the Username of the instance?

When creating AWS EC2, it only supports key pair for verification. As for username, Windows server: `Administrator`. For username of Linux server, please see [accounts-OS](/stack-accounts.md).

#### What is the username and password of database?

The username and password of database is stored on your instance, please refer to this section [Username and password](/stack-accounts.md).

#### How to enable the root user of Linux?

By default, the root account is not enabled on AWS, but we can find a way to enable it.

Refer to this section [Linux Connect](/server-login.md).

#### How to upload Files to instance?

For Windows Server, you can Copy local files and Paste them to Server.  
For Linux Server, you can use **SFTP** tools to login Server, and upload files.

#### Can the image be refunded?

For image billed hourly, the system generates bills based on the actual usage. Hence, on refund is allowed. If you don't use image, please delete the image or stop EC2.

For image billed annually, you can refund for the remaining time of image A when you change image A to image B.

#### What should I do if the EC2's IP address changes after it restarts?

It is recommended to change to a static IP or set up a DNS provided by AWS for the server.

#### Does Websoft9 have free image?

We do not offer free images on AWS. If you want to use our deployment package freely, please download our automation script via [Github](https://github.com/websoft9) and deploy it via Ansible.

#### Is there a difference between the Github script deployment and the AWS cloud market image deployment for Websoft9?

The deployment results are the same, but the deployment is different.

#### How to list all products of Websoft9 on AWS Marketplace?

Link to [Websoft9 Products](https://aws.amazon.com/marketplace/seller-profile?id=c639a579-182c-4d30-8578-4d4d89fba658) or search keyword "Websoft9" on AWS Marketplace.

#### Can the image on instance be replaced?

No.

#### What's the difference between instance store and EBS?

An instance store provides temporary block-level storage for your instance.Instance store is ideal for temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content, or for data that is replicated across a fleet of instances, such as a load-balanced pool of web servers. 

EBS provides block level storage volumes.You can mount these volumes as devices on your EC2 instances, or detach it from EC2 without losing data.

#### Can I create EC2 OS username?

There is only default username when creating EC2. You can use the default users name to log in to the system, and then create more usernames on your own.