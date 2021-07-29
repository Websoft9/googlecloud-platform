# Snapshots and Images

The reason we put snapshots and image together is that there is a certain relationship between the two, and even an alternate relationship.

## Relationship

Key connection between snapshots and image are as follow:

* A snapshot can be created based on the disk.

  A snapshot is a "photographing" of a disk. As the name suggests, it is to back up the data of a disk at a certain point in time. It is a backup method.

* A image can be created based on a snapshot, but the image cannot be directly converted into a snapshot.

* Based on the image, you can create an instance directly, and you can create a image directly based on the instance.  

Summary: (volume --> snapshot) --> (image - instance)


## Create Snapshots

For AWS, to create Snapshots based on the volume.

1. Login to the AWS console and open EC2 Dashboard.  

2. Open 【ELASTIC BLOCK STORE】>【Volumes】 and choose volume to create Snapshot.
   ![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-createsnapshot-websoft9.png)

3. Name the snapshot before creating.

## Create Image

As mentioned before, image can be created based on snapshots, and instance.

### Instance to Image

1. Login to AWS console.  

2. Choose the instance, and open 【Actions】>【Image】>【Create image】.
![img](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-ec2toimage-websoft9.png)   

3. Follow the prompts to complete it.

### Snapshots to Image

1. Login to the Aws console and open EC2 Dashboard.  

2. Open 【ELASTIC BLOCK STORE】>【Create Snapshot】 and list all snapshots.
3. Choose from the list of snapshots and create image based on it.
   ![Snapshots](https://libs.websoft9.com/Websoft9/DocsPicture/en/aws/aws-snapshot-websoft9.png)