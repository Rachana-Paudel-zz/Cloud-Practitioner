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

<img src="start_lab.PNG" alt="start_lab" style="height: 100%; width:45%; padding-right:10px"/>
<img src="start_ready.PNG" alt="start_lab" style="height: 100%; width:45%;"/>

+   At the top of these instructions, choose `AWS`

+   Arrange the AWS Management Console tab so that it displays along side these instructions. Ideally, you will be able to see both browser tabs at the same time so that you can follow the lab steps.

## Creating a bucket in Amazon S3

+   In this task, I create an S3 bucket and configure it for static website hosting.[`click to learn`](https://awseducate.instructure.com/courses/815/modules/items/14096)

<img src="bucket_creation.PNG" alt="start_lab" style="height: 100%; width:45%;padding-right:10px;"/>
<img src="bucket_create.PNG" alt="start_lab" style="height: 100%; width:45%;"/>



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

<img src="static_web.PNG" alt="static web" style="height: 100%; width:45%; padding-right:10px"/>
<img src="static_Web_hosting.PNG" alt="static web" style="height: 100%; width:45%;"/>

## 3. Uploading content to your bucket
+   In this task, upload the static files to your bucket.
[`Learn to upload`](https://awseducate.instructure.com/courses/815/modules/items/14096)



<img src="add_file_3.PNG" alt="object" style="height: 100%; width:45%;"/>
<img src="uploaded.PNG" alt="object" style="height: 100%; width:45%;"/>



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

+ Notice that the index.html file is listed in the `Failed to delete` pane. 

This confirms that your policy is working and preventing the website's files from being deleted.

+   Choose `Close` to return to the `Objects` tab.


##  7. Updating the website

[`Learn `](https://awseducate.instructure.com/courses/815/modules/items/14096)

<img src="" alt="report" style="height: 100%; width:45%; padding-right:10px"/>





## 8. Exploring file versions

<img src="show_version.PNG" alt="report" style="height: 100%; width:100%"/>

