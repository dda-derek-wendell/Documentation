---
sectionclass: h2
sectionid: marketo_lead_source
parent-id: marketo_documentation
number: 2900
title: Set up Person Source with a Triggered Campaign 
---
>This configuration is **optional** but is highly recommended.  
{:.warning}

>Assigning a custom person source to records created by Dodge Link enables:  

●  Administrators to identify records added by the Dodge Prospecting feature    
●  Smart lists to filter using the Person Source and other attributes    

>Before beginning, you will need to:  

●  Obtain administrator access to the Marketo instance. The Marketo instance should support Custom Object triggers. See [Marketo Documentation](https://docs.marketo.com/display/public/DOCS/Trigger+Off+Custom+Object+Changes)    
●  Decide on a custom source name.  It is recommended to use **Dodge Link**
●  Identify the name for the custom contact object associated with the lead. These will be referred to as **Custom Contact** in the Triggered Campaign instructions.    

>Description:  

The Dodge Contact custom object will have a field for __Source__.  When the record is created using Prospecting, the value of **Source** will be __Y__.  For records that previously existed or were created by any other process, the Source value will be blank.  Where the field **Source** in Dodge Contact equals **Y** the trigger will add a **Person Source = Dodge Link** or whatever name used.
