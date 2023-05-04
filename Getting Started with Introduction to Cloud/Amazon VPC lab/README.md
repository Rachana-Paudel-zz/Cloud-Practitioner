### Amazon VPC lab

####    Lab 5: Creating a Virtual Private Cloud

#####   Task 1: Creating a VPC
A VPC is a virtual network that is dedicated to your Amazon Web Services (AWS) account. It is logically isolated from other virtual networks in the AWS Cloud. You can launch AWS resources, such as Amazon Elastic Compute Cloud (Amazon EC2) instances, into the VPC. You can configure the VPC bymodifying its IP address range and can create subnets. You can also configure route tables, network gateways, and security settings.

+   In the AWS Management Console, on the Services  menu, choose VPC
+   In the left navigation pane, choose Your VPCs.
+   A default VPC is provided so that you can launch resources as soon as you start using AWS. There is also a shared VPC that you use later in the lab. However, you now create your own Lab VPC.

The VPC will have a Classless Inter-Domain Routing (CIDR) range of 10.0.0.0/16, which includes all IP address that start with 10.0.x.x. It contains more than 65,000 addresses. You later divide the addresses into separate subnets.
+   Choose Create VPC.

+   Under Resources to create, choose VPC only.