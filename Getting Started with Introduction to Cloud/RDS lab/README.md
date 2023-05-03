### Lab 4: Creating an Amazon RDS Database
####    Task 1: Creating an Amazon RDS database
+   On the Services  menu, choose RDS.

+   Choose Create database

+   Under Engine options, select  MySQL.

+   The options include several use cases, ranging from enterprise-class databases to Dev/Test systems. In the options, you might notice Amazon Aurora. Aurora is a MySQL-compatible system that was re-architected for the cloud. If your company uses large-scale MySQL or PostgreSQL databases, Aurora can provide enhanced performance.

+   In the Templates section, select  Dev/Test.
+   In Availability and durability section, choose  Single DB instance.
+   In the Settings section, configure the following options:

DB instance identifier: `inventory-db`
Master username: `admin`
Master password: `lab-password`
Confirm password: `lab-password`

+   In the DB instance class section, configure the following options:

Select  Burstable classes (includes t classes).
Select db.t3.micro
+   In the Storage section, configure the following options:

Storage type: Select General Purpose SSD (gp2).
Allocated storage: Enter 20 GiB.
In the Connectivity section, configure the following option: 

Virtual private cloud (VPC): Lab VPC
+   In the Connectivity section, for Existing VPC security groups, choose the X on default to remove this security group. Then choose the dropdown list, and select DB-SG to add it.

+   Scroll to the Monitoring section, and clear (deselect) the Enable Enhanced monitoring option.
+   Scroll to the Additional configuration section, and choose  to expand it. 
+    For Initial database name, enter inventory
+   At the bottom of the page, choose Create database
	You should receive this message: Creating database inventory-db.

