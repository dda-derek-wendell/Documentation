---
sectionclass: h2
sectionid: disableduplicate
parent-id: documentation
number: 1300
title: Disable Duplicate Detection
---

>The user has two options to disable duplicate detection altogether or to disable it for the only the user who installed the package (this is the user new fields will be added as)
1) Disable for all users
**Click Setup**
In left nav search type "Duplicate Rules"
**Click Duplicate Rules** which is located under "Duplicate Management"
For each duplicate rule, click the rule name and select "Edit"
**Click Deactivate** this will disable the rule
**Click Back to List: Duplicate Rules** and repeat for "Contact" and "Lead" rules.

>2) Disable for single installation user
For each duplicate rule, click the rule name and select "Edit"
Under conditions, add a condition with "Current User: Username", "not equal to", and the salesforce username (login) of the user that installed the package.
Repeat for all applicable rules
