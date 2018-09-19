---
sectionclass: h2
sectionid: setleadsource
parent-id: documentation
number: 1350
title: Add Dodge Link as Account or Lead Source with Process Builder (Optional)
---
>This configuration is **optional** and is availability on 1.3 and higher versions in Salesforce.  
{:.warning}

>Adding Dodge Link as the source for each account, contact and lead created by the Salesforce package could be helpful so it is a recommended best practice.  It will help with identifying records added by Dodge Prospecting and creating views on Accounts, Contacts and Leads 

>There are 3 required steps if your version is 1.2, otherwise  there are only 2 steps.

●  For those on version 1.2 you must upgrade to 1.3 or the latest version.  Contact Dodge Customer Care to get the upgrade Link.  Follow the provided instructions to install and configure the instructions. 
●  1.41 will add a new picklist value
●  1.42 Create workflow in Process Builder 
●  You will need Identify the Salesforce package's names for the custom account, contact, and lead objects (Setup > Objects > list of objects for the installed package). These will be referred to as **Custom_Account, Custom_Contact,** and **Custom_Contact_Lead** objects in the Process Builder instructions.  

 
