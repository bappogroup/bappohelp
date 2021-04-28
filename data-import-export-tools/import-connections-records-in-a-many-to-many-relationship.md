---
description: >-
  How to upload (import) CSV files with connections (records in a many-to-many
  relationship)
---

# Import Connections \(records in a many-to-many relationship\)

### Upload Connections in Many-to-Many Relationships

It is important to understand that when you create a many-to-many relationship, Bappo automatically creates a new table \(or object\) to store all the connections. Each connection is a unique record in this table. For example, if two parents have two children, you need to create four connections. Bappo stores these connections in the connections table like this.[![](https://downloads.intercomcdn.com/i/o/70257703/2c3dd3ee6f03817430308fd1/Screen+Shot+2018-08-02+at+12.23.38+pm.png)](https://downloads.intercomcdn.com/i/o/70257703/2c3dd3ee6f03817430308fd1/Screen+Shot+2018-08-02+at+12.23.38+pm.png)

Therefore, connections between records that have a many-to-many relationship need to be uploaded and downloaded separately. Many-to-many relationships are common. You will note that each field name includes the extension \[name\]. Take note that the names must be unique. If there are multiple children with the name "Peter", the upload tool would not be able to tell which Peter to select. Alternatively you could download the records, which will include both the \[id\] and \[name\] of each child.  Id is always a unique field so you can instead use \[id\] to match children to parents.

To view the format of your table, we suggest you download the table first .

1. To access CSV file migrations, you click on the down arrow next to the Space name at the top of the left panel in user mode.
2. Select 'CSV Migration' 
3. Click on the download icon next to the object name you want to download the records from. For example: 'ParentChildConnection'.

[![](https://downloads.intercomcdn.com/i/o/70259415/f1db2bff72f8d472c0187131/Screen+Shot+2018-08-02+at+12.51.58+pm.png)](https://downloads.intercomcdn.com/i/o/70259415/f1db2bff72f8d472c0187131/Screen+Shot+2018-08-02+at+12.51.58+pm.png)

4. Replace the '1000' next to ‘Amount of records to download’ with the number of records you want to download and click on the accept mark[![](https://downloads.intercomcdn.com/i/o/70259666/fd6d3251c3b64e6f5c0dec66/Screen+Shot+2018-08-02+at+12.54.37+pm.png)](https://downloads.intercomcdn.com/i/o/70259666/fd6d3251c3b64e6f5c0dec66/Screen+Shot+2018-08-02+at+12.54.37+pm.png)

5. Your records will be downloaded as a '.csv' file which should appear on your screen. 

6. When you open this file, you will see a table with the fields in the object as headings and your records underneath

Once your field headings are ready you can enter the data into the table. Once you're done, just save it as a CSV file.[![](https://downloads.intercomcdn.com/i/o/70259885/96743db1c6f9fb3761b83bc2/Screen+Shot+2018-08-02+at+1.00.20+pm.png)](https://downloads.intercomcdn.com/i/o/70259885/96743db1c6f9fb3761b83bc2/Screen+Shot+2018-08-02+at+1.00.20+pm.png)

The records that you want to connect, must already exist in the database. If they don't exist yet, you will have to enter or upload them first.

Now that your table is ready, you can start to upload the CSV file.[![](https://downloads.intercomcdn.com/i/o/70260123/be673201e075058c6d516e36/Screen+Shot+2018-08-02+at+1.04.34+pm.png)](https://downloads.intercomcdn.com/i/o/70260123/be673201e075058c6d516e36/Screen+Shot+2018-08-02+at+1.04.34+pm.png)

1. In user mode, click on the download icon next to the Space name at the top of the left panel
2. Select 'CSV Migration' 
3. Click on the up arrow icon next to the object name you want to upload the records to. For example 'ParentChildConnection'
4. Select the CSV file you would like to upload from your file manager
5. An import file with the validation result will now appear on your screen. Review the file. If all the records are correct, press 'Upload All'.
6. Once the upload is complete you will see the upload result and a "Completed" message.
7. You can close this message by clicking the X in the upper left corner.

### WARNING:

 Do not upload connections that already exist in your database. The upload file will create a duplicate connection. One way to prevent this from happening is to make the name of the record unique.

