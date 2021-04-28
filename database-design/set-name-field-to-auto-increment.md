# Set Name Field to Auto Increment

When you create a new Object, you automatically generate a Name field. By default this field will be where you enter the names of your records. This will always be the first field that appears on your form when you create a new record or when you search for a record.

But you can edit this field to better suit the nature of your Object. As with any other field you can:

* Edit the Field Name
* Set a Default Value to the Field
* Set the field to be required
* Set the field to be unique

Most importantly, you can also set the field to auto-increment

For example, if the object is an invoice, this field can be an automatically generated invoice number \(e.g. INV0001\)

To change this field to automatically generate an invoice number.

1. In the [Database Builder](http://help.bappo.com/database-use/switch-between-user-mode-and-design-mode) on the left, select the name field e.g. ‘Invoice Name’
2. Find the checkbox ‘Convert this field to Auto Increment’ and turn it on
3. Enter a prefix e.g. INV
4. Select the starting number. You can include zeros in front of the number e.g. 0001
5. Click on ‘Convert’
6. You should see the ‘Conversion succeeded!’ message
7. Exit the ‘Edit Field’ popup and your records will auto increment

### You can always revert the auto increment back to text

1. In the [Database Builder](http://help.bappo.com/database-use/switch-between-user-mode-and-design-mode) on the left, select the name field e.g. ‘Invoice Name’
2. Turn on the checkbox ‘Convert the field back to text’ 
3. Enter a new field name. This may be the same as the existing field name.
4. Click on ‘Convert’
5. You should see the ‘Conversion succeeded!’ message
6. Exit the ‘Edit Field’ popup and your records will auto increment

Note: You will notice that the technical name of the field has not changed. All forms will show the new name, but developers will use the technical name during coding.

