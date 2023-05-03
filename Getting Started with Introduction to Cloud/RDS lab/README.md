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

####    Task 2: Configuring web application communication with a database instance
+   On the Services  menu, choose EC2.
+   In the left navigation pane, choose Instances.
In the center pane, there should be a running instance that is named App Server.
+   Select the check box for the App Server instance.
+   In the Details tab, copy the Public IPv4 address to your clipboard.
+   Open a new web browser tab, paste the IP address into the address bar, and then press Enter.
+   Choose  Settings.
+   Return to the AWS Management Console, but do not close the application tab. (You will return to it soon.)
On the Services  menu, choose RDS.
+   In the left navigation pane, choose Databases.
+   Choose inventory-db.
+   Scroll to the Connectivity & security section, and copy the Endpoint to your clipboard.
It should look similar to this example: inventory-db.crwxbgqad61a.rds.amazonaws.com
+   Return to the browser tab with the inventory application, and enter the following values:

    +       For Endpoint, paste the endpoint you copied earlier.
    +   For Database, enter inventory
    +   For Username, enteradmin
    +   For Password, enter lab-password
    +   Choose Save.
    The application will now connect to the database, load some initial data, and display information.
+   You can use the web application to   Add inventory,  edit, and  delete inventory information.
+   Insert new records into the table. Ensure that the table has 5 or more inventory records before submitting your work.