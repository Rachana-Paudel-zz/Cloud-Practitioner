### Lab 2: Introduction to Amazon EC2

####    Task 1: Launching your EC2 instance

+   In the AWS Management Console on the Services menu, choose EC2.
+   In the left navigation pane, choose EC2 Dashboard to ensure that you are on the dashboard page.
+   Choose Launch instance, and then select Launch instance.

#####   Step 1: Name your EC2 instance
+   In the Name and tags section, for Name, enter Web-Server
+   Choose the Add additional tags link.
+   From the Resource types dropdown list, ensure that both Instances and Volumes are selected.
<img src="step1.PNG" alt="" style="height::100%; width: =100%;"   >

#####   Step 2: Choose an Amazon Machine Image (AMI)
An Amazon Machine Image (AMI) provides the information required to launch an instance, which is a virtual server in the cloud. An AMI includes the following:

+   A template for the root volume for the instance (for example, an operating system or an application server with applications)
+   Launch permissions that control which AWS accounts can use the AMI to launch instances
+   A block device mapping that specifies the volumes to attach to the instance when it is launched.

The Quick Start list contains the most commonly used AMIs. You can also create your own AMI or select an AMI from the AWS Marketplace, an online store where you can sell or buy software that runs on AWS.
+   Locate the Application and OS Images (Amazon Machine Image) section. It is just below the Name and tags section.
+   In the AMI Machine Image (AMI) box, notice that Amazon Linux 2 AMI is selected by default. Keep this setting.

<img src="s2.PNG" alt="" style="height::100%; width: =100%;"   >