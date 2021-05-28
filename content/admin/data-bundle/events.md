---
weight: 11
title: "Events"
layout: redirect
---

**Purpose**: Different events could be created in the Upkip Administration. They are built with a specifically designed expression language that supports some limited amount of operations and functions. Event triggers when defined expression in it returns true. Events trigger the warnings and notifications. 

When Tags of type Int have defined MIN/MAX values, events are created automatically if tag value is outside of the defined region.
### Create Events manually
Precondition: User with role Administrator is logged in Upkip Administration. Select menu **Events**.

- List of events in the administration is shown

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.088.png)

*Figure 86: Upkip Administration - Events*

Click **New** button to create new Event.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.089.png)

*Figure 87: Upkip Administration - Events - New event fields*

Enter to create Event:

- **Name** of the event
- **Expression** of the event. Expressions are defined by using Function from **+Add Function** and Tags by **+Add Tag.** To create an expression are used some operators:
   - Math operations: -, +, \*, /, ^, sqr
   - Logical operations: Use & or  |
   - Comparison operators: <, >, <=, >=, =, != 
   - User parentheses () to set the order of operations;
- **Expression parameters** is possible to define with Name, Type (Number, Boolean, String, DateTime) and Value.

To save event click **Add** button. 

- The created event appears in the list of events by (Name and Expression)


### Search and Add Tag
After selecting built in function and it includes some tag, tag can be searched and selected from the organization Tag list.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.090.png)

*Figure 88: Upkip Administration - New event - add expression with tag*

Click on **Add Tag** button. 

- The form for searching and selecting Tag is opened.
##### Search Tag from all tags
![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.091.png)

*Figure 89: Upkip Administration - new event - search tag*

1) Filter tags by Name or Display Name and click Search. Tags are filtered.
1) Select tag from the list. The **Select Tag** button is enabled.
1) Click **Select Tag** button
   1. Selected tag appears in the entered expression. 

##### Select tag from Organization tree
Tag can be searched and selected through organization tree with departments and machines.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.092.png)

*Figure 90: Upkip Administration - new event - search tag from organization tree*

1) From the SELECT TAG form click on tab Organization. 
- At the left organization tree with departments and machines is shown.
1) Expand the organization tree with departments, select some machine
- The list of tags for selected machine is listed on the right side
1) Filter the tags by typing in the Filter field
1) Select tag from the list. The Select Tag button is enabled.
1) Click **Select Tag**
- Selected tag appears in events expression field.

Event could be saved by clicking **Save**.

### Create Events and Warnings from Tag limits
**Purpose**: It is possible when adding a Tag to specify Min or Max values of the tag. It is usually used for numeric tags. To configure the tag limits follow the steps below:

Login and go to **Organization Items** tab.

Browse and locate the machine of interest and click on it.

To the right open **Tags** tab and use the **Filter** field to locate the target tag or click on the button **Edit** at to bottom to edit the tag. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.093.png)

*Figure 91: Upkip Administration - Select machine tag*

- Form for editing the tag is opened

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.094.png)

*Figure 92: Upkip Administration - Add tag limits with create warnings*

Enter the tag value limits for **Min and/or Max.** You can input only one limit or both. 

Bellow the Min and Max fields there are checkboxes: 

- **Create warning** – check both and click **Save** 
  - Automatically will be created a relevant **Events** and **Warnings** which can be seen in the **Events** and **Warnings lists**.

Select Menu **Warnings** and search in the list – e.g. Temp-Pump1

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.095.png)

*Figure 93: Upkip Administration - Automatically created warnings from tag limits*

- **Two warnings** of type **Alarm** are created automatically for MIN and MAX values of the tag.

Select Menu **Events** and search in the list – e.g. Temp - Pump1

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.096.png)

*Figure 94: Upkip Administration - Automatically created events from tag limits*

- **Four events** are created automatically, **start and stop event** for MIN and for MAX values of the tag.
### Edit Tag with Delete warning checked
When editing again TAG with MIN and MAX Limits and already created warnings and events is possible to check **Delete warning** and click **Save**. 

- **Delete warning** – appears for previously defined limits that already has warning and event. If selected this checkbox and click Save, will delete the **relevant Warning, Event and any Notifications attached to the event.**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.097.png)**

*Figure 95: Upkip Administration - Edit tag with checked Delete warning*

- All relevant warnings, events automatically created and notifications created by them will be deleted on saving Tag with checked Delete warning checkboxes.


