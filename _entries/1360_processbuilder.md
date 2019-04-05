---
sectionclass: h3
sectionid: processbuilder
parent-id: setleadsource
number: 1360
title: Process Builder
---
>This step is recommended but not a requirement. 
>If your package version is 1.2 install the 1.3 upgrade in order to use this fefature.  See below step 1.16
>This step will create 3 seperate Process Builder processes.  There will be a process for Accounts, Contacts, and Leads.  These processes will run when a new account , contact or lead is created from Dodge Prospecting.
The processes will Add the value **"Dodge Link"** to the Account Source or Lead Source field <!--and change the owner of the record to the user that created the record from Dodge Prospecting. -->

Suggested names for each Process Builder Process are:
<br>Accounts = **Set Source <!--and Owner --> on Accounts to Dodge Link** 
<br>Contacts = **Set Source <!--and Owner --> on Contacts to Dodge Link**
<br>Leads = **Set Source <!--and Owner --> on Leads to Dodge Link** 

**Please Note:** These processes only affect newly created records. Records previously created by Dodge Prospecting will not be affected.
{:.warning}

>Setup > type "process builder" in Quick Find > click **Process Builder** (under Workflow & Approvals)  

><p style="color:red">
Start by creating the Process for Accounts<br>
When creating Contact and Lead processes, the process names will be "Set Source <!--and Owner -->on Contact to Dodge Link" or "Set Source<!-- and Owner--> on Lead to Dodge Link" accordingly./p>
  
>Click **New** button
  ・Process Name: **Set Source <!--and Owner on -->Account to Dodge Link**  
  ・The process starts when: **a record changes**<br>
  ・    Click **Save**  
  
![Process_Builder_NewProcess]({{ site.baseurl }}/img/1500/Process_Builder_NewProcess.png)  

>Click **Add Object**  
  ・    Object: Choose **Dodge_Account**   
  ・    Start the process: **only when a record is created**    
  ・    Click **Save**  

![Process_Builder_AddObject]({{ site.baseurl }}/img/1500/Process_Builder_AddObject.png)

><p style="color:red">
 When creating Contact and Lead processes and at the below step to "Add Criteria" you will change the criteria name to Dodge Contact Source = Y or Dodge Lead Source = Y accordingly</p>

>Click **Add Criteria**   
  ・Criteria Name: **Dodge Account Source = Y** 
  ・Criteria for Executing Actions: **Conditions are met**  
  ・Set Conditions: Choose the Source field.  
      ・Field = Source   
      ・Operator = Equals  
      ・Type = String  
      ・Value = Y  
  ・Conditions **All of the conditions are met (AND)**  
  ・Click **Save**  

![Process_Builder_AddCriteria]({{ site.baseurl }}/img/1500/Process_Builder_AddCriteria.png)

<p style="color:red">
When you are creating the Contact or Lead process and at the below step to to add an action you will change the record type to Dodge_Contacts or Dodge_Contact_Lead and the field to Contacts or Leads accordingly</p>
  
>Click **Add Action**  
  ・    Action Type: **Update Records**  
  ・    Action Name: **Update Source<!-- and Owner**  -->
  ・    Record Type: **Select a record related to the dodge_Dodge_Account_c**  
  ・    Choose Field : **Account**  Do not choose any value with ">" like **Account > | Contact > | Lead >**  
  ・    Click **Choose**  

![Process_Builder_SelectRecord]({{ site.baseurl }}/img/1500/Process_Builder_SelectRecord.png)  

>  ・   Criteria for updating records: **No criteria - just update the records!**  
  ・    Field: For Accounts, choose **Account Source**.  For Contacts or Leads, choose **Lead Source**  
  ・    Type: **Select Picklist**  
  ・    Value: **Choose Dodge Link**
  
  <!--Add another Field
  ・    Field: **Owner ID**. 
  ・    Type: **Select Formula**  $User.Id** -->
  
  ![Process_Builder_Actions]({{ site.baseurl }}/img/1500/Process_Builder_Actions.png)

>Click **Save**  
>Review your entries, and click **Activate**  

><p style="color:red">
   Repeat the Process Builder instructions to create processes Contacts, and Leads </p>
  
