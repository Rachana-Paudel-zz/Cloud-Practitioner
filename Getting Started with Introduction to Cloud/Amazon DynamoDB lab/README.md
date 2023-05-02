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

####    Task 2: Adding Data
Each table contains multiple items. An item is a group of attributes that is uniquely identifiable among all of the other items. Items in DynamoDB are similar in many ways to rows in other database systems. In DynamoDB, there is no limit to the number of items that you can store in a table.
Each item consists of one or more attributes. An attribute is a fundamental data element, something that does not need to be broken down any further. For example, an item in a Music table contains attributes such as song and artist. Attributes in DynamoDB are similar to columns in other database systems, but each item (row) can have different attributes (columns).

When you write an item to a DynamoDB table, only the primary key and sort key (if used) are required.  Other than these fields, the table does not require a schema, which means that you can add attributes to one item that may be different than the attributes on other items.
+   Select Explore items on the left side navigation pane.

+   Click the radio button next to Music to select the table you created.

+   Click Create item.

+   Add in the following values.