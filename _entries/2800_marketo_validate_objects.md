---
sectionclass: h2
sectionid: marketo_validate_objects
parent-id: marketo_documentation
number: 2800
title: Validate Marketo Custom Objects in Customer Portal
---

>After you've created the custom objects, their fields, and approved those objects, you may now validate your installation.

>In the Dodge Link Portal's **Instance Fields** validation tool, click Refresh Configuration.  
This tool will compare your Marketo configuration to the expected configuration.
When the page refreshes the correctly configured fields and objects will display with a green checkmark and success message.   
Incorrectly configured fields and objects will display with a red X and error message.  

![test image]({{ site.baseurl }}/img/2800/field_validation.jpg)

>**NAME_NOT_FOUND** could be that you did not create that field.  This is perfectly fine.

>The Dodge custom objects inthe Dodge Link Portal should look like this.  
<br>Either Ok or One or more fields is not configured is acceptable

![test image]({{ site.baseurl }}/img/2800/custom_object_validation.jpg)


>To make a field channge after the object has been approved follow these 4 steps
<br>1. Delete the field
<br>2. Approve the Dodge custom object
<br>3. Add a New Field
<br>4. Approve the Dodge custom Object


>The Marketo integration will not work correctly until all objects and fields are correctly configured.
Once the custom objects and fields are correctly configured, you are ready to use your data integration!
