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

#####   Step 3: Choose an instance type
Amazon EC2 provides a wide selection of instance types that are optimized to fit different use cases. Instance types comprise varying combinations of CPU, memory, storage, and networking capacity and give you the flexibility to choose the appropriate mix of resources for your applications. Each instance type includes one or more instance sizes so that you can scale your resources to the requirements of your target workload.

In this step, you choose a t2.micro instance. This instance type has 1 virtual CPU and 1 GiB of memory.
+   Keep the default instance type, t2.micro.

#####   Step 4: Configure a key pair
Amazon EC2 uses public key cryptography to encrypt and decrypt login information. To log in to your instance, you must create a key pair, specify the name of the key pair when you launch the instance, and provide the private key when you connect to the instance.

In this lab, you do not log in to your instance, so you do not require a key pair.
+   In the Key pair (login) section, from the Key pair name - required dropdown list, choose Proceed without a key pair.

<img src="s3.PNG" alt="" style="height::100%; width: =100%;"   >

#####   Step 5: Configure the network settings

You use this pane to configure networking settings.

The virtual private cloud (VPC) indicates which VPC you want to launch the instance into. You can have multiple VPCs, including different ones for development, testing, and production.

 

+   In the Network settings section, choose Edit.

+   From the VPC - required dropdown list, choose Lab VPC.

The Lab VPC was created using an AWS CloudFormation template during the setup process of your lab. This VPC includes two public subnets in two different Availability Zones.

+   In the Network settings section, for Security group name - required, enter Web Server security group
+   To delete the existing SSH rule, next to Security group rule 1, choose Remove.

<img src="s4.PNG" alt="" style="height::100%; width: =100%;"   >

#####   Step 6: Add storage

Amazon EC2 stores data on a network-attached virtual disk called Amazon Elastic Block Store (Amazon EBS).

You launch the EC2 instance using a default 8 GiB disk volume. This is your root volume (also known as a boot volume).
+   In the Configure storage pane, keep the default storage configuration.

<img src="s5.PNG" alt="" style="height::100%; width: =100%;"   >

#####   Step 7: Configure advanced details
+   Expand the Advanced details pane.
+   From the Termination protection dropdown list, choose  Enable.
+   Copy the following commands, and paste them into theIn the User data text box.


`#!/bin/bash
yum -y install httpd
systemctl enable httpd
systemctl start httpd
echo '<html><h1>Hello From Your Web
Server!</h1></html>' > /var/www/html/index.html`

The script does the following:

+   Install an Apache web server (httpd)
+   Configure the web server to automatically start on boot
+   Activate the Web server
+   Create a simple web page
 


<img src="s7.PNG" alt="" style="height::100%; width: =100%;"   >

#####   Step 8: Launch an EC2 instance

+   In the Summary section, choose Launch instance.

+   Choose View all instances

The instance appears in a Pending state, which means that it is being launched. It then changes to Running, which indicates that the instance has started booting. There will be a short time before you can access the instance.

The instance receives a public Domain Name System (DNS) name that you can use to contact the instance from the Internet.

Next to your Web-Server, select the  check box. The Details tab displays detailed information about your instance.

 To view more information in the Details tab, drag the window divider upward.
 Review the information displayed in the Details, Security and Networking tabs.

 

+   Wait for your instance to display the following:

Note: Refresh if needed.
+   Instance State:  Running
+   Status Checks:   2/2 checks passed