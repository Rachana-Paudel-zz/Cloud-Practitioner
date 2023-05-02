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

Artist: Pink Floyd
Song: Money

These are the only required attributes, but you can now add additional attributes.
+   To create an additional attribute, click the Add new attribute button.

+   In the dropdown list, choose String.

+   A new attribute row is added.

+   For the new attribute, replace NewValue withAlbum and in the Value column enter The Dark Side of the Moon.

+   Add another new attribute by choosing the Add new attribute button.
+In the dropdown list, choose Number.

+For the new attribute, replace NewValue with Year and in the Value column replace 0 with 1973.
+   Choose Create item to store the new item with its four attributes.


+   The item appears in the Items returned pane in the console.
+   Next, follow the previous steps and use the following attributes to create a second item:

`Attribute Name`	`Attribute Type`	`Attribute Value`
Artist	              String	          John Lennon
Song	              String	          Imagine
Album	              String	          Imagine
Year	              Number	          1971
Genre	              String	          Soft rock

Note that this item has an additional attribute called Genre. Adding this attribute is an example of each item being capable of having different attributes without having to pre-define a table schema.

Follow the previous steps and use the following attributes to create a third item:

Attribute Name	Attribute Type	Attribute Value
Artist             String	       Psy
Song	           String	       Gangnam Style
Album	           String	       Psy 6 (Six Rules), Part 1
Year	           Number	        2011
LengthSeconds	   Number	        219


Once again, this item has a new LengthSeconds attribute that identifies the length of the song. The ability to include this attribute demonstrates the flexibility of a NoSQL database.
There are also faster ways to load data into DynamoDB, such as using AWS Data Pipeline, programmatically loading data, or using one of the free tools available on the internet.

####    Task 3: Modifying an Existing Item
+   From the list of items, select the row where the Artist is Psy.

+   Choose the Actions menu, and select Edit item.

+   Change the Year Number from 2011 to 2012.
+   Choose Save changes.

The item is now updated

####    Task 4: Querying the Table
+   Choose Explore items in the left navigation pane.

+   Select Music.

+   If Scan/Query items is not already expanded, choose the arrow  to expose the Scan and Query options
+   Choose Query.

Fields for the Artist (which is the same as partition key) and Song (which is the same as sort key) are now displayed.

+   Enter the following details:

Artist (Partition key): Psy
Song (Sort key): Equal to Gangnam Style
+   Choose Run.
+   Choose the Scan option.

+   Choose the arrow  to expand Filters.

+   Enter values for the scan filter:

For Enter attribute name, enter YearChange String to Number.
Condition: Select Equal to
For Enter value, enter 1971
Choose Run.
Only the song released in 1971 is displayed.


