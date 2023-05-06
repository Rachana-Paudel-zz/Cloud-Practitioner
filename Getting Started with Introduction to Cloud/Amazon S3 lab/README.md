### Lab 7: Hosting a Static Website
####    Task 1: Creating a bucket in Amazon S3
+   In the AWS Management Console, on the Services menu, choose S3.

+   Choose Create bucket

An S3 bucket name is globally unique, and all AWS accounts share the namespace. After you create a bucket, no other AWS accountsin any AWS Regions can use the name of that bucket unless you delete the bucket.

Thus, for this lab, you use a bucket name that includes a random number, such as website-123.
+   For Bucket name, enter website-<123> and replace <123> with a random number.

Public access to buckets is blocked by default. Because the files in your static website will need to be accessible through the internet, you must permit public access.

+   First Under ObjectOwnership choose ACL enabled.

+   Choose Bucket owner preferred.

+   Under Block Public Access settings for this bucket. Clear the check box for Block all public access, and then select the box that states I acknowledge that the current settings may result in this bucket and the objects within becoming public.

+   Under Tags Select Add tag and enter the following:

    +   Key: Department
    +   Value: Marketing
    You can use tags to add additional information to a bucket, such as a project code, cost center, or owner.

    Choose Create bucket

In the Buckets section, choose the name of your new bucket.

Choose the Properties tab.

You will now configure the bucket for static website hosting.

+   Scroll to the Static website hosting panel.

+   Choose Edit

+   Configure the following settings:

    +   Static web hosting: Choose Enable.

    +   Hosting type: Choose Host a static website.
    +   Index document: Enter index.html

    Note: You must enter this value even though it is already displayed.
    +   Error document: Enter error.html
+   Choose Save changes

+   In the Static website hosting panel under Bucket website endpoint, choose the link.

You receive a 403 Forbidden message because you have not yet configured the bucket permissions. Keep this tab open in your web browser so that you can return to it later.

You have configured your bucket to host a static website.


####    Task 2: Uploading content to your bucket
In this task, you upload the static files to your bucket.

+   Right-click each of the following links, and download the files to your computer:
Ensure that each file keeps the same file name, including the extension.

  +   index.html
    +   script.js
    +   style.css

   

Return to the Amazon S3 console, and choose the Objects tab.
Choose Upload
Choose Add files
Choose the three files that you downloaded.
+   Choose Upload
Your files are uploaded to the bucket.