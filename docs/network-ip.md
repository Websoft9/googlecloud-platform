# Public IP Address

## View

1. Login to AWS console.  

2. Choose the instance, and you can see the **Public IP** and **Public DNS**.
   ![View IP](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-getip-websoft9.png)  

3. If the instance does not have a public IP address entry (or is empty), you need to refer to the next section to mount a public IP address.


## Mount

If the created instance does not have a public IP address, as long as there is a free (or newly purchased) public IP address, the AWS console can mount the public network IP address to the instance.The specific steps are as follows: 

1. Login to AWS console.  

2. Choose the instance and open 【Actions】>【Networking】>【Manage IP Addresses】.
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-manageip-websoft9.png)

3. Click 【Allocate an Elastic IP】.
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-assignip-websoft9.png)

4. Follow the prompts to complete the action.