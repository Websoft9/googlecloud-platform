# Domain Name

General skill such as applying for a domain name and resolving domain names will not discussed in this document.

Here we introduce a more useful domain feature of AWS: AWS provides DNS services for each instance.

## DNS for EC2

AWS provides public public DNS services for each instance.

When the instance is configured with a dynamic IP address, the IP address may change each time the instance is restarted. As a result, the domain name needs to be re-resolved, which brings unnecessary trouble to the operation and maintenance. AWS's DNS function can help us avoid this problem.

1. Login to AWS console and open 【Instance】>【Description】.
   ![view DNS](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-getip-websoft9.png)  

2. Copy the public DNS.

## Route 53

Route 53 is the platform for applying domain, domain resolution and management. You can use Route 53 to register domain names, transfer existing domains, route traffic for your domains to your AWS and external resources and check the health of your resources.

1. Login to AWS console and choose Route 53 in 【Networking & Content Delivery】.
   ![Route 53](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-route53-websoft9.png)
2. Start to manage domains.
   ![Route 53](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-route53start-websoft9.png)
