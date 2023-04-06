## Getting started with cloud storage.

+ In this module we learn about basic storage domain and AWS course storage services.
+   It is broken into four following sections.
Click [Getting Started with Cloud Storage](https://awseducate.instructure.com/courses/815) to start learning.

<img src="Concept_Storage.PNG" alt="Storage module" style="height: 100%; width:45%; padding-right:10px"/><img src="Concept_Storage2.PNG" alt="Storage module" style="height: 100%; width:45%;"/>

#### Starting here with Amazon Simple Storage Service (Amazon S3) 

##### After completing this lab, I will be able to do the following:

+   Create a bucket in Amazon S3.
+   Configure a bucket to host a    static website.

+   Upload content to a bucket.

+   Allow Enable public access to bucket objects.

+   Securely share a bucket object by using a presigned URL.

+ Secure a bucket by using a bucket policy.

+ Update the website.

+ View object versions in the Amazon S3 console.

## Getting Started learning pathway

### 1. Accessing the AWS Management Console
+    At the top of these instructions, choose `Start Lab` to launch your lab.
[Getting Started with Cloud storage](https://awseducate.instructure.com/courses/815/modules/items/14096) to start learning.

<img src="start_lab.PNG" alt="start_lab" style="height: 100%; width:45%; padding-right:10px"/><img src="start_ready.PNG" alt="start_lab" style="height: 100%; width:45%;"/>

+   At the top of these instructions, choose `AWS`

+   Arrange the AWS Management Console tab so that it displays along side these instructions. Ideally, you will be able to see both browser tabs at the same time so that you can follow the lab steps.

## Creating a bucket in Amazon S3

+   In this task, I create an S3 bucket and configure it for static website hosting.[`click to learn`](https://awseducate.instructure.com/courses/815/modules/items/14096)

<img src="bucket_creation.PNG" alt="start_lab" style="height: 100%; width:45%;padding-right:10px;"/><img src="bucket_create.PNG" alt="start_lab" style="height: 100%; width:45%;"/>



## 2.Configuring a static website on Amazon S3
##### configure the bucket for static website hosting.

+   Scroll to the <b>Static website hosting</b> panel.

+ Choose `Edit`.

+ Configure the following settings:

    +   Static web hosting: Choose `Enable`.
    +   Hosting type: Choose `Host a static website`.
    +   Index document: Enter `index.html`
    +   Error document: Enter `error.html`
##### Note: You must enter index.html and error.html even though they are already displayed.

+ Choose `Save changes`

+ In the Static website hosting panel under Bucket website endpoint, choose the link.

You receive a 403 Forbidden message because you have not yet configured the bucket permissions. Keep this tab open in your web browser so that you can return to it later.

You have configured your bucket to host a static website.

<img src="static_web.PNG" alt="static web" style="height: 100%; width:45%; padding-right:10px"/><img src="static_Web_hosting.PNG" alt="static web" style="height: 100%; width:45%;"/>

## 3. Uploading content to your bucket
+   In this task, upload the static files to your bucket.
[`Learn to upload`](https://awseducate.instructure.com/courses/815/modules/items/14096)



<img src="add_file_3.PNG" alt="object" style="height: 100%; width:45%;"/><img src="uploaded.PNG" alt="object" style="height: 100%; width:45%;"/>



## 4. Turning on public access to the objects
+   Objects that are stored in Amazon S3 are private by default. This setting helps keep your organization's data secure.

In this task, you make the uploaded objects publicly accessible so users can view your website.

First, confirm that the objects are currently private.

[`Learn more`](https://awseducate.instructure.com/courses/815/modules/items/14096)

<img src="error.PNG" alt="object" style="height: 100%; width:100%;"/>



## 5. Securely sharing an object using a presigned URL

######    When you need to temporarily and securely share an object with a person or group of people, you can create a presigned URL. When you create the URL, you must configure how long the URL will be valid. Then, you can share this URL with the users who should have access to the object.

[`Learn more`](https://awseducate.instructure.com/courses/815/modules/items/14096)

<img src="new_report.PNG" alt="report" style="height: 100%; width:45%;"/><img src="predesignurl.PNG" alt="report" style="height: 100%; width:45%;"/>

##  6. Using a bucket policy to secure your bucket

###### You want to protect your website files and make sure that no one can delete them. To do this, you apply a bucket policy that denies delete privileges on your website files.

+   Return to the Amazon S3 console, and choose the `Permissions` tab.
+ Under Bucket policy, choose `Edit`
+ Copy the following policy text. In the Policy text editor, replace the existing policy text with this text:
<i>[`code`](https://awseducate.instructure.com/courses/815/modules/items/14096)</i>
Note: Your bucket name will be different. Be sure to use the name of the bucket that you created.

+   Choose `Save changes`

+   Return to the  the Object tab

+ Select  index.html.

+ Choose `Delete`.

+ In the Delete objects panel, enter delete to confirm that you want to remove this file.

+ Choose `Delete objects`

+ Notice that the index.html file is listed in the `Failed to delete` pane. This confirms that your policy is working and preventing the website's files from being deleted.

+   Choose `Close` to return to the `Objects` tab.


##  7. Updating the website

[`Learn`](https://awseducate.instructure.com/courses/815/modules/items/14096)

<img src="website.PNG" alt="report" style="height: 100%; width:45%; padding-right:10px"/>

## 8. Exploring file versions

<img src="show_version.PNG" alt="report" style="height: 100%; width:100%"/>

### AWS Educate's Cloud Challenges!
   Here is some information about Cloud storage, regions,availability and redundancy.

+ Click to [learn](https://awseducate.instructure.com/courses/543
)
<img src="availability_redundancy.PNG" alt="storage" style="height: 100%; width:45%; padding-right:10px;"/><img src="availability.PNG" alt="storage" style="height: 100%; width:45%"/><img src="regions.PNG" alt="storage" style="height: 100%; width:100%"/>

+   Types of Data in the Cloud

<img src="data1.PNG" alt="Data" style="height: 100%; width:45%; padding-right:10px"/>
<img src="data2.PNG" alt="Data" style="height: 100%; width:45%; "/>


+   Working of Simple Storage Service(S3) with users data and assesment.
<img src="Bucket.PNG" alt="Working" style="height: 100%; width:45%; "/><img src="challenges.PNG" alt="Working" style="height: 100%; width:45%; "/>
+   Assessement
<img src="assesment.PNG" alt="Assessement" style="height: 100%; width:100%; "/>

##  Intoduction to Storage

+ Benefits of Cloud Storage
<img src="benefits_of_cloud_storage.PNG" alt="Benefits" style="height: 100%; width:100%; "/>

+ Types of Cloud storage
<img src="types_of_Storage.PNG" alt="Benefits" style="height: 100%; width:100%; "/>

+ choosing right storage
<img src="choosing_storage.PNG" alt="right_storage" style="height: 100%; width:100%; "/>

+ Storage use cases
  + block storage and object storage
  <img src="block_storage_usecase.PNG" alt="right_storage" style="height: 100%; width:45%;padding-right:10px; "/><img src="object_Storage_usecase.PNG" alt="right_storage" style="height: 100%; width:45%; "/>

+ AWS core storage services
  + Amazon Elasic Block Store
  + Amazon Elastic File System
  + lsAmazon Simple Storage Service


## Introduction to Amazon S3

+ Basic S3 workflow
  + move data into Amazon S3
  + Store data as objectsin Amazon S3
  + Use data in applicaions
+ Object level storage
+ Active and archive storage
<img src="active_archieve_storage.PNG" alt="Active and archive storage" style="height: 100%; width:100%; "/>
+ Amazon storage S3 storage class
<img src="s3_storage classes.PNG" alt="S3 storage" style="height: 100%; width:100%; "/>
+ Amazon S3 storage classes use cases
<img src="s3usecase.PNG" alt="use cases" style="height: 100%; width:100%; "/>
+ Amazon S3 costs

<img src="S3costs.PNG" alt="S3 costs" style="height: 100%; width:100%; "/>


##   Create a bucket
+ create a bucket
+ configure the bucket
  + choose a reason
  + object ownershio and access
  + bucket versioning
  + tags

+ upload objects
   + unlimited data
    + 5 TB object limit
    + 160 GB upload limit from the console
+  upload objects-multipart upload  
<img src="multipartupload.PNG" alt="Multipart" style="height: 100%; width:100%; "/>
+ work with objects
<img src="workwithobjects.PNG" alt="Object work" style="height: 100%; width:100%; "/>
+ delete objects and buckets
<img src="deletebuckets.PNG" alt="Object delete" style="height: 100%; width:100%; "/>

+ Additional features
  + lifecycle rules
  <img src="lifecyclerules.PNG" alt="lifecycle rules" style="height: 100%; width:100%; "/>
  + replication rules 
  <img src="replicationrules.PNG" alt="replications" style="height: 100%; width:100%; "/>

  <img src="crossregion.PNG" alt="cross_region" style="height: 100%; width:45%;padding-right:10px; "/> <img src="sameregion.PNG" alt="replications" style="height: 100%; width:45%; "/>

  + security

<img src="bucketsecurity.PNG" alt="bucketsecurity" style="height: 100%; width:45%; "/><img src="iampolicies.PNG" alt="iampolicies" style="height: 100%; width:45%; "/>
<img src="bucketpplicy.PNG" alt="bucketpplicy" style="height: 100%; width:45%; "/><img src="bucketencryption.PNG" alt="replications" style="height: 100%; width:45%; "/>

### Moving large amount of data into Amazon S3
+ S3 Transfer Acceleration
+ AWS Snowcone
+ AWS Snowball
+ AWS Snowmobile




### `End of Cloud storage.`