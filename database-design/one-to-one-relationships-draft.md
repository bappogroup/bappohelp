---
description: How to create one-to-one relationships between records
---

# One-to-one relationships - draft

By creating a relationship between your Objects you are able to connect records together and use your data more effectively.

One-to-One Relationship

One-to-one relationships occur when there is exactly one record in the first table that corresponds to one record in the related table. A real life example is "Spouse" in monogamous cultures. Each person can have only one spouse.  
A country may issue drivers licenses to its citizens. Each citizen is only allowed to have one drivers license. In this case the object "Citizen" and the object "Drivers License" will have a one-to-one relationship.  
  
Another common use of one-to-one relationships is when you want to extend a table, but not all records need the extended information. For example you may have "Additional Information" for an "Invoice". If only some of the invoices have additional information, it is better to create a separate object for the additional information. 

A useful trick in Bappo is to link Users in a one-to-one relationship to other objects that contain information about the users \(e.g. Employees or Customers\). This relationship comes in handy when you want to create forms that auto-fill the user's information.

Here's how to do this:

**Add New Relationship**

1. If you are in User Mode, go to 'Modify this App' by clicking the panel on the bottom left of the screen.
2. In the the Design Panel on the left, click on the Object to which you want to add a field with a relationship.
3. Under the subheading RELATIONSHIPS, click on '+ Add New Relationship'.
4. In the dropdown box in the popup, select the Target Object that is in this relationship.
5. Create the relationship using the example above by changing both connections to 'One'

Let's use the case of an 'Invoice' that may have additional 'Invoice information'.

* Each Invoice connects with **One** Invoice Information
* Each Invoice Information connects with **One** Invoice

**Rename the Connections**  
If the name of the object is not descriptive of the name of the connection, you can rename the connection

1. In the the Design Panel on the left, click on the Object that contains the relationship.
2. Under the subheading RELATIONSHIPS, click on the relationship. It is flagged with a chain link.
3. The relationship details will appear in a pop up screen with the names of the connections underlined. You can edit each of the two connections.
4. Save the new names

Let's use the case of an 'Invoice' that may have additional 'Invoice information'.

* Each Invoice connects with **One** Invoice Information
* Each Invoice Information connects with **One** Invoice

Now \(using this example\), if you create a new record in the 'Invoice' Object. If you go into the record, you will see a Tab with the name \(let's say 'Additional Invoice Information'\) you have given the relationship. You will be able to add a new record with the additional invoice information and link it to this new record.

