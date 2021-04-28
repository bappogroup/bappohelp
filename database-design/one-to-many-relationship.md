# One-to-Many Relationship

### One to Many Relationship

One-to-many relationships are the most common type of database relationship. They occur when each record in Object A corresponds to one or more records in Object B, but each record in Object B corresponds to only one record in Object A. For example, the relationship between a Company table and an Employee table would likely be a one-to-many relationship, because each employee has only one company, but each company has many employees. This one-to-many design helps eliminate duplicated data.

Whenever add a field to an object, and then associate that field with another object, you have created a many-to-one relationship between these two objects.

Here's how to create a one-to-many relationship:

1. Click on 'Add New Relationship' in the [Database Builder](http://help.bappo.com/database-use/switch-between-user-mode-and-design-mode) under any one of the two Objects you want to link.
2. In the dropdown box in the popup, select the Target Object for the relationship.
3. Create the relationship by changing the 'One' and 'Many' where necessary and click on 'Create'. It should look something like this:

* Each Employee connects with **One** Company
* Each Company connects with **Many** Employees 

You will notice that a data entry field will now appear on the form of the object on the **Many** side. If you expand that object in the Database Builder, you can also see the field among the other fields under the object.

If you also want to see the connection when you look at the object on the **One** side, you can switch on a Tab that shows all the records in Object B that are associated with Object A. 

1. Click on the relationship in the [Database Builder](http://help.bappo.com/database-use/switch-between-user-mode-and-design-mode) on the left, 
2. Turn the tab on by turning on the slider that says 'Show a tab of "Object B" in "Object A" view.'

Using this example: You will now be able to see a tab of the **Many** Object \(Employees\) when you click on a record in your **One** Object \(Companies\).

**Change the Display name of the tab in the relationship \('One' Side\)**

The name of your Object is usually a main table that you can use in different ways. If you create a relationship you may want to change the name of that connection so it displays something different from the Object name when you view the tab in the connected Object.

Read [best practices for naming Objects](http://help.bappo.com/faq-and-tips/tips/best-practices-for-naming-objects) to understand this concept further.

1. Click on the relationship in the [Database Builder](http://help.bappo.com/database-use/switch-between-user-mode-and-design-mode) on the left
2. The relationship details will appear in a pop-up screen with the names of the connections underlined. This will change the display name of the tab and/or the display name of the field.

* Each Employee connects with **One** Company as \_\_Staff\_\_\_\_
* Each Company connects with **Many** Employees as \_\_\_\_\_\_\_\_\_\_

3. Then click on 'Update'.

Once you have created a record for a new company, you'll be able to open the record. The main tab will show the main form with all the company details. Next to the "Company" tab, you will see a tab for "Staff". If you click on this tab, it will show you all the staff associated with this company. You will also be able to create new staff, by clicking on the button "Create New Staff".

**Change the field name of the Relationship \(Many side\)**

By changing the **Many** side of the relationship you are changing the field that it creates. Using the same example as above, when you create a One-to-Many relationship it will create a field in the Employee records called 'Company'. Let's say you want to change this to 'Employer' or maybe 'Previous Employer' etc. You would change the **Many** line:

* Each Employee connects with **One** Company as \_\_\_\_\_\_\_\_\_
* Each Company connects with **Many** Employees as \_\_\_Employer\_\_\_\_\_

You can create as many of these relationships as you need and be able to use the same Object \(as an example 'Companies'\) for numerous fields on the form. When you go to create a record for an Employee, you may have three different fields 'Previous Employer', 'Current Employer' and 'Employer of Choice'. These are technically the same relationship using the same connected records from the Object 'Companies' but with different headings/meanings for each selection.

