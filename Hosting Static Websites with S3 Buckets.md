# Overview of Amozon Simple Storage Service(S3)

Amazon Simple Storage Service (Amazon S3) is an object storage service that is it is used to store and protect any amount of data and other variety of use cases, including data lakes, websites, mobile applications, backup and restore, archives, enterprise applications, IoT devices, and big data analytics. In order to meet your unique business, organizational, and compliance requirements, Amazon S3 offers management features that allow you to optimize, organize, and configure access to your data. Amazon S3  stores data as objects( a file and any metadata that describes it) within buckets.

To store  data in S3, you create a bucket first and choose a bucket name and AWS Region,then you upload your data to that bucket as objects in Amazon S3.It has the following features:

* You can use the storage management features of Amazon S3 to control costs, adhere to regulatory requirements, lessen latency, and store multiple unique copies of your data for compliance purposes.

* Using S3 object lambda and event notification to transform data and start workflows to automate a variety of other processing tasks at scale.

* Features for managing and auditing access to your buckets and objects are available in Amazon S3. S3 buckets and the objects contained within them are by default private. Only the S3 resources you create are accessible to you.

* You can better understand, analyze, and optimize your storage at scale by using the features it provides to help you gain visibility into your storage usage.

## How to host a static website on AWS using S3 buckets 
1. Log in to the console at https://console.aws.amazon.com/s3/ 9tis lab requires demo codes for the static website, which is available at the demo codes folder)

2. Click on create bucket 

3. In bucket name, enter a unique name for your bucket which should be DNS-compliant( Your bucket name cannot be changed after bucket is created

4. In Region, choose the AWS Region closest to you for low latency.

5. Under Object Ownership, choose either Acls Disabled( bucket owner automatically owns and has full control over every object in the bucket) or Acls enabled( here  bucket owner owns and has full control over new objects).

6. Select the Block Public Access settings you want to apply to the bucket under Bucket settings for Block Public Access(it is recommended to tick all boxes and block public access unless you are hosting a public website on the bucket). In our case, we are hosting public static website which should be accessible to the public so uncheck the boxes and click on agree.

7. Click on advanced options if you want to enable object lock(this is optional) so we would ignore it and just go ahead and create the bucket.

## Uploading the demo codes to the bucket

1. Click on the newly created bucket and navigate to Upload

2. You either drag and drop the demo files or select from your files directly.

3. After dropping your files, click on upload(wait for few minutes as it can take time to upload depending on the volume of uploaded code)
