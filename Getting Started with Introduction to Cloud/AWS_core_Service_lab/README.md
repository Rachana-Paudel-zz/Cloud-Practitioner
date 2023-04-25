####    Lab 1: Introduction to Amazon Simple Storage Service (Amazon S3)

After completing this lab, we will know how to:

+   Create a bucket in Amazon S3
+   Add an object to a bucket
+   Manage access permissions on an object and a bucket
+   Create a bucket policy
+   Use bucket versioning
 ion of these instructions.

#####   Task 1: Creating a bucket

+   At the upper left of the AWS Management Console, on the Services menu, choose S3.
+   Choose Create bucket
 
+   In the General configuration section, enter the following as the Bucket name: reportbucket(NUMBER)
    Example bucket name: reportbucket987987

+   Leave Region at its default value.    

#####   Task 2: Uploading an object to the bucket
+   Right-click the following link: new-report.png. Choose Save link as, and save the file to your desktop.
+   In the S3 Management Console, find and select the bucket name that starts with reportbucket.
+   Choose Upload
+   Choose Add files
+   Browse to and select the new-report.png file that you downloaded previously.
+   At the bottom of the page, choose Upload
+   Oue file is successfully uploaded when the green bar indicating Upload succeeded appears.

+   In the Upload: status section in the upper right, choose Close

#####   Task 3: Making an object public
+   In the reportbucket overview page, on the Objects tab, locate the new-report.png object, and choose the new-report.png file name.
The new-report.png overview page opens. The navigation in the upper left updates with a link to return to the bucket overview page.

+   In the Object overview section, locate and copy the Object URL link.

The link should look similar to the following: https://reportbucket987987.s3-us-west-2.amazonaws.com/new-report.png

+   Open a new browser tab and paste the object URL link into the address field, and then press Enter.
You receive an Access Denied error because objects in Amazon S3 are private by default.

Now that you've confirmed that the default security of Amazon S3 is private, you test how to make the object publicly accessible.

+   Keep the browser with the Access Denied error open, and return to the web browser tab with the S3 Management Console.
+   We should still be on the new-report.png Object overview tab.
+   In the upper right, choose the Object actions dropdown menu, you will notice that Make public via ACL is greyed out.
+   In the upper left of the page, choose the reportbucket name in the navigation to go back to the main reportbucket overview page.
+   Choose the Permissions tab.
+   We need to allow the use of ACLs first. Under Object Ownership choose Edit.
+   Choose ACLs enabled.
+   Choose Bucket owner preferred.
+   Choose the  check box next to I acknowledge that ACLs will be restored.
+   Choose Save Changes
+   Under Block public access (bucket settings), choose Edit to change the settings.
+   Clear the check box for the Block all public access option, and then leave all other options cleared.
+   Choose Save changes
+   A dialogue box opens asking you to confirm your changes. Enter confirm in the field, and then choose Confirm

A message that says Successfully edited Block Public Access settings for this bucket. displays at the top of the window.

+   Choose the Objects tab.
+   Choose the new-report.png file name.
+   At the upper right on the new-report.png overview page,choose the Object actions dropdown menu, and select Make public.
 Notice the warning: When public read access is enabled and not blocked by Block Public Access settings, anyone in the world can access the specified objects. This warning reminds you that if you make the object public, then everyone in the world will be able to read the object. 

+   Choose Make public and you should see the green banner Successfully edited public access at the top of the window.
+   In the upper right, choose Close to return to the new-report.png object overview.
+   Return to the browser tab that displayed Access Denied for the new-report.png object, and refresh the page.

+   Close the web browser tab that displays your new-report.png image, and return to the tab with the Amazon S3 Management Console.

#####   Task 4: Testing connectivity from the EC2 instance

+   On the Services menu, choose EC2.
+   On the EC2 Dashboard, under the Resources section, choose Instances (running).
+   Select the  check box for Bastion Host and choose Connect
+   In the Connect to instance window, select the Session Manager tab for the connection method.
+   Choose Connect
+   In the bastion host session, enter the following command to change to the home directory (/home/ssm-user/):
`cd ~`

The output returns you to the command prompt.

+   Enter the following command to verify that you are in the home directory:
`pwd`
The output should be as follows:
`/home/ssm-user`

+   Enter the following command to list all of your S3 buckets. 
`aws s3 ls`
  The output should look similar to the following:

  `2020-11-11 22:34:46 reportbucket987987`

+ In the following command, change (NUMBER) at the end of the reportbucket name to the name of the bucket you created. Enter your adjusted command to list all the objects in your reportbucket. 
`aws s3 ls s3://reportbucket(NUMBER)`

+   The command looks similar to the following: aws s3 ls <b>s3://reportbucket987987<b>

The output should look like the following:

`2020-11-11 15:46:34      86065 new-report.png`

+   Enter the following command to change directories into the reports directory.

`cd reports`
The output returns you to the command prompt.

+   Enter the following command to list the contents of the directory.
`ls`

The output shows some files created in your reports directory to test the application.

`dolphins.jpg files.zip report-test.txt  report-test1.txt report-test2.txt report-test3.txt  whale.jpg`

+   In the following command, change (NUMBER) at the end of the reportbucket name to the name of the bucket you created. Enter your adjusted command to see if you can copy a file to the S3 bucket.

`aws s3 cp report-test1.txt s3://reportbucket(NUMBER)`

The command looks similar to this: <b>aws s3 cp report-test1.txt s3://reportbucket987987<b>

The output indicates an upload failed error. This error occurs because you have read-only rights to the bucket and do not have the permissions to perform the PutObject action.

+   Leave this window open. and go back to browser tab with the AWS console.
In the next task, you create a bucket policy to add the PutObject permission.