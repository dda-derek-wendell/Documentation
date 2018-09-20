---
sectionclass: h3
sectionid: processbuilder
parent-id: setleadsource
number: 1360
title: Process Builder
---
>This step will create 3 seperate Process Builder processes.  There will be one for Accounts, Contacts, and Leads.  Each process will select the Dodge Link pick list value and add it to the Account Source or Lead Source when a record is created by Dodge Prospecting. 

Sugested names for each Process Builder Process are:
<br>Accounts = **Set Source on Account to Dodge Link** 
<br>Contacts = **Set Source on Contacts to Dodge Link**
<br>Leads = **Set Source on Leads to Dodge Link** 

**Note:**  Once these processes are activated **Dodge Link** will be added to newly created records. Records previously created by Dodge Prospecting will continue to have a blank value in Account or Lead Source unless they are updated manually.  
{:.warning}

>Setup > type "process builder" in Quick Find > click **Process Builder** (under Workflow & Approvals)  

>Click **New** button
Start by creating the Process for Accounts<br>
**<p style="color:red"Change the process name accordingly when creating process for contacts and leads</p>**
  ・Process Name: **Set Source on Account to Dodge Link**  
  ・The process starts when: **a record changes **
  ・Click **Save**

![Process_Builder_NewProcess]({{ site.baseurl }}/img/1500/Process_Builder_NewProcess.png)  

>Click **Add Object**  
  ・    Object: Choose **Dodge_Account**   
  ・    Start the process: **only when a record is created**    
  ・    Click **Save**  

![Process_Builder_AddObject]({{ site.baseurl }}/img/1500/Process_Builder_AddObject.png)

>Click **Add Criteria**   
  ・Criteria Name: **Custom Object Source = Y** (This name is not important)  
  ・Criteria for Executing Actions: **Conditions are met**  
  ・Set Conditions: Choose the Source field.  
      ・Field = Source   
      ・Operator = Equals  
      ・Type = String  
      ・Value = Y  
  ・Conditions **All of the conditions are met (AND)**  
  ・**Save**  

![Process_Builder_AddCriteria]({{ site.baseurl }}/img/1500/Process_Builder_AddCriteria.png)


>Click **Add Action**  
  ・    Action Type: **Update Records**  
  ・    Action Name: **Update Source**  
  ・    Record Type: **Select a record related to the (custom object)**  
  ・    Choose **Account | Contact | Lead** depending on process being built. Do not choose **Account > | Contact > | Lead >**  
  ・    Click **Choose**  

![Process_Builder_SelectRecord]({{ site.baseurl }}/img/1500/Process_Builder_SelectRecord.png)  

>  ・    Criteria for updating records: **No criteria - just update the records!**  
  ・    Field: For Accounts, choose **Account Source**.  For Contacts or Leads, choose **Lead Source**  
  ・    Type: **Picklist**  
  ・    Value: choose the picklist value created  

![Process_Builder_Actions]({{ site.baseurl }}/img/1500/Process_Builder_Actions.png)

>Click **Save**  
Review your entries, and click **Activate**  
Repeat the Process Builder instructions to create processes for Accounts, Contacts, and Leads  
