---
description: Good object names help maximise your database performance.
---

# Best practices for naming objects

The best way to name an object is to think what name can best describe the records you are to create.

Here is an example scenario: When you need a list of travel destinations, e.g. 'Australia', 'India' etc, then you might want to create an object called 'Countries' rather than 'My travel destinations'. By doing this, other objects can now create relationships with the 'Countries' object, and now your ‘Countries’ can be used in a variety of ways.

Let's say, you now have 3 objects in the system, 'Travellers', 'Travel Agencies' and ‘Countries’. Now 'Travellers' can create a relationship with ‘Countries’. This is where you can use display names to make it easier for users to understand the purpose of the field. You could use 'Travel destination' as the display name, so when you create a record you will be selecting your travel destination from your list of Countries.  
As another example of using the same object ‘Countries', you could create a relationship between 'Travel Agencies' and 'Countries' with 'Available Market' as the display name. Therefore when you create a record in that object, you will be selecting the ‘Available Market’ from the list of Countries. [![](https://downloads.intercomcdn.com/i/o/71651026/07cf2f130f0accee44904bdf/image.png)](https://downloads.intercomcdn.com/i/o/71651026/07cf2f130f0accee44904bdf/image.png)

The display name of a relationship can be edited by clicking on the relationship in the Design Panel \(‘relates to one...' button\), then edit the 'as' part.  


