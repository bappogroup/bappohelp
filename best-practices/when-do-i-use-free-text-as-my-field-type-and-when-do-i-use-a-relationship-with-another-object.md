---
description: >-
  This article will help you decide when to use relationships with another
  object or when users should use free text type their own data.
---

# When do I use free text as my field type, and when do I use a relationship with another object?

The general rule is that if you use the data more than once it is best to store the data in a separate object and refer to the data.  
This also makes it easier to create reports or workflows. 

The challenge is that in most instances the data must already be available and updated in the other object. Often there is an infinite range of possibilities, and you don't want to create a record for every single possibility. In this case you would choose a text field type.

Here are three examples:

1. Let's say you deal with staff who all live locally, but you also want to know their place of birth. You may create a table that includes all the suburbs in your home town as a drop-down for their current address. But you don't want to add every town on earth to capture their place of birth; you would make their place of birth a free text.
2. Or let's say you're building a database with your customer records, you will probably create a separate object called "Customers" and upload or enter all your customer data in that table. This will allow you to always refer to that record in all your transactions or activities that relate to that customer. And you can create reports about that customer or other per customer reports, like sales per customer or complaints per customer etc. But let's say you have thousands of cash customers and you deal with every customer only once or twice, and although you may search on that field, you don't need any report on that field. In that case, you may make the Customer field a free text field.
3. In the third example you may be a recruiter who wants to connect job-seekers with new employers. You may have a database of employers that your job-seekers can choose from, but you also want to know who their current employer is, to make sure you don't accidentally introduce them to their current employer. The "Choice of Employer" field should relate to the "Employer" object. But the "Current Employer" field may be free text, because you don't want a table with every single employer in the world. An alternative may be to give them the option of either choosing their current employer from you "Employer" object and give them an "Other" option, if their current employer is not in your database.

