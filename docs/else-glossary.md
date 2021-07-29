# Glossary

#### AWS Management Console

A graphical interface to manage compute, storage, and other cloud resources.

#### AWS CLI

AWS Command Line Interface (AWS CLI), is a unified downloadable and configurable tool for managing AWS services. Control multiple AWS services from the command line and automate them through scripts.

#### EC2

Amazon Elastic Compute Cloud (Amazon EC2) provides scalable computing capacity in the Amazon Web Services (AWS) cloud. Using Amazon EC2 eliminates your need to invest in hardware up front, so you can develop and deploy applications faster. You can use Amazon EC2 to launch as many or as few virtual servers as you need, configure security and networking, and manage storage. Amazon EC2 enables you to scale up or down to handle changes in requirements or spikes in popularity, reducing your need to forecast traffic.

#### DNS

DNS (domain name server) is a service that routes internet traffic to websites by translating friendly domain names like www.example.com into the numeric IP addresses like 192.0.2.1 that computers use to connect to each other.

#### AWS Marketplace

A web portal where qualified partners market and sell their software to AWS customers. AWS Marketplace is an online software store that helps customers find, buy, and immediately start using the software and services that run on AWS.

#### Port

A port is an endpoint of communication in computer networking. This can be hardware port, a logical port, or both. TCP and UDP ports are identified by their port number (an integer from 0 to 65535).

#### Secure Shell (SSH)

A cryptographic network protocol for operating network services securely over an unsecured network based at the application layer and transport layer.

#### Secure Shell key pair (SSH key pair)

A set of security credentials that you use to prove your identity electronically. A key pair consists of a private key and a public key.

If the public key has been stored in the Linux instance, you can use the private key to log in to the instance through the local computer or other instances without a password by using SSH commands or related tools.

#### Snapshot

A copy of data on a disk at a certain time point. There are two types of snapshots, automatic snapshots and user-created snapshots.

#### SFTP

SFTP (SSH File Transfer Protocol) is a secure file transfer protocol. It runs over the SSH protocol. It supports the full security and authentication functionality of SSH.

#### Security Group

A security group implements access controls for instance, specifying the communication scope of instance. You can define different access control rules for a security group, and these rules take effect for all instance added to this security group. By default, a security group allows all data packets that are sent out from instance in it, and instance in the same security group can access each other.

#### Amazon EBS

Amazon Elastic Block Store (Amazon EBS) provides block level storage volumes for use with EC2 instances. You can mount these volumes as devices on your instances. EBS volumes that are attached to an instance are exposed as storage volumes that persist independently from the life of the instance. You can create a file system on top of these volumes, or use them in any way you would use a block device (such as a hard drive). You can dynamically change the configuration of a volume attached to an instance.

#### Amazon EC2 instance store

An instance store provides temporary block-level storage for your instance. This storage is located on disks that are physically attached to the host computer. Instance store is ideal for temporary storage of information that changes frequently, such as buffers, caches, scratch data, and other temporary content, or for data that is replicated across a fleet of instances, such as a load-balanced pool of web servers.

#### Amazon S3
Amazon S3 is a repository for internet data. Amazon S3 provides access to reliable, fast, and inexpensive data storage infrastructure. It is designed to make web-scale computing easier by enabling you to store and retrieve any amount of data, at any time, from within Amazon EC2 or anywhere on the web. Amazon S3 stores data objects redundantly on multiple devices across multiple facilities and allows concurrent read or write access to these data objects by many separate clients or application threads. You can use the redundant data stored in Amazon S3 to recover quickly and reliably from instance or application failures.

#### Data disk

A data disk is a managed disk that's attached to an instance to store application data, or other data you need to keep. Data disks are registered as SCSI drives and are labeled with a letter that you choose. Each data disk has a maximum capacity of 32,767 gibibytes (GiB). The size of the instance determines how many data disks you can attach to it and the type of storage you can use to host the disks.

#### OS disk

Every instance has one attached operating system disk. That OS disk has a pre-installed OS, which was selected when the instance was created. This disk has a maximum capacity of 2,048 GiB.

#### Route 53

A web service you can use to create a new DNS service or to migrate your existing DNS service to the cloud.

#### Volume

A fixed amount of storage on an instance. It's the same with disk.