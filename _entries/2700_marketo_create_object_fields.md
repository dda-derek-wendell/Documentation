---
sectionclass: h2
sectionid: marketo_create_object_fields
parent-id: marketo_documentation
number: 2700
title: Create Marketo Custom Fields
---


>This step Dodge fields wills be created in each of the custom objects in Marketo. 

In the Dodge Link Portal, click on a one of the custom object names (dodge_Account_c, dodge_Contact_c, dodge_Project_c, dodge_Role_c) to expand the list of fields. 

>The **status** will show with errors until the fields are created and the object is approved.  
{:.warning}
>Do not approve the object until you are finished creating the fields.    
{:.warning}
![test image]({{ site.baseurl }}/img/2700/instance_fields_fields.jpg)

>Marketo will automatically create fields for **Created At**, **Marketo GUID**, and **Updated At**

![test image]({{ site.baseurl }}/img/2700/marketo_automatic_fields.jpg)

>In Marketo, Click on **Marketo Custom Objects** in the sidebar Admin menu, select one of the Dodge custom objects, and then Click **Fields** at the top  
Click **New Field**   

![test image]({{ site.baseurl }}/img/2700/click_fields.jpg)


>Create the **leadId** field that will link the custom object to the **Person** object.  The Person object was formerly called the Lead object. Each Dodge custom object needs this leadId field. Repeat this step for the remaining custom objects. 

>It is important to know that the API Name is **case sensitive**.
>Be sure to use **Data Type: link** and **Dedupe Field: Yes** 
> dodge_Account and dodge_Contact will each have 1 more field marked at **Dedupe Field: Yes**.  Otherwise do not make any other field **Dedupe Field: Yes**   
{:.warning}

![test image]({{ site.baseurl }}/img/2700/leadId_field.png)

>Create the rest of the fields using the Customer Portal's Instance Fields tool as a guide for API names and Types.
<br> Which Dodge fields are created in each object is personal preference.  Marketo has a limit of 47 fields per custom object. 

>Remember the API Name is **case sensitive**  
   
{:.warning}

![test image]({{ site.baseurl }}/img/2700/new_field.jpg)

>**Dedupe Field: or dodge_Projects and dodge_Roles Look Like**
![test image]({{ site.baseurl }}/img/2700/set_dodge_project_id_dedupe.jpg)
<br>
![test image]({{ site.baseurl }}/img/2700/dodge_projects_dedupe_fields.jpg)
<br>
![test image]({{ site.baseurl }}/img/2700/set_dodge_role_id_dedupe.jpg)
<br>
![test image]({{ site.baseurl }}/img/2700/dodge_role_dedupe_fields.jp

>After creating all the fields , you must approve the object.
On the **Marketo Custom Objects** tab, in the **Custom Object Actions** menu, click **Approve Object**  
Click the **Approve** button to confirm

![test image]({{ site.baseurl }}/img/2700/approve_object.jpg)

>Repeat steps for each Dodge custom object
{:.warning}
