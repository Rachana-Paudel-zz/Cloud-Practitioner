### Lab 3: Introduction to Amazon DynamoDB

####    Task 1: Creating a New Table
+   In the AWS Management Console, choose Services, and then choose DynamoDB.

+   Choose Create table

+   For Table name, enter Music

+   For Partition key, enter Artist and leave String selected.
+   For Sort key - optional, enter Song and leave String selected.

+   Under Settings select Customize settings then configure the following

#####   Read capacity
+   Provisioned capacity units: 10

#####   Write capacity
Provisioned capacity units: 2

 Amazon DynamoDB has two read/write capacity modes for processing reads and writes on your tables:

On-demand
Provisioned (default, free-tier eligible)

The read/write capacity mode controls how you are charged for read and write throughput and how you manage capacity. You can set the read/write capacity mode when creating a table or you can change it later.
Your table will use default settings for indexes.
+   Choose Create table.

The table is created in less than 1 minute.