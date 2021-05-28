---
title: "Warnings"
date: 2021-05-20T15:44:20+03:00
draft: false
weight: 12
layout: redirect
---

Precondition: Log in the Upkip Administration. Select menu **Warnings**. 

**Purpose**:
- The warnings are created with different severity: **Information, Warning or Alarms.** 
- Warnings have **start and stop events.** See [Create Events](/admin/data/#events)
- Warnings could be created automatically when entering Tag limits.  [Automatically create warnings and events](/admin/data/#create-events-and-warnings-from-tag-limits)
- Warnings could be visualized on the dashboard to indicate that some tags values are not in the limits. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.098.png)

*Figure 96: Upkip Administration - Warnings*


### Create or Edit Warning
Click on the **New** button. 

- The form for creating warning is opened.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.099.png)

*Figure 97: Upkip Administration - New warning fields*

Enter in the form the following data:

- **Name** of the warning 
- **Severity** – select the severity of the warning from drop down list - **Information, Warning, Alarm**
- Select the **start event** from the list with events
- Select the **stop event** from the list with events
-  Click **Add**.
- The created warning appears in Warnings list with its **Severity and Name.**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.100.png)

*Figure 98: Upkip Administration - Warnings with different severity*

Select some warning from the list and lick Edit.

- Form for editing warning is opened. 

Warning can be edited by changing Name, Severity, Start and Stop event. Click Save to save to edited warning.

- The edited warning is saved

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.101.png)

*Figure 99: Upkip Administration - Edit Warning fields*

### Delete Warning
Select some warning and click **Delete**.

- There appears confirmation warning. If confirm click Delete button.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.102.png)

*Figure 100: Upkip Administration - Delete warning*

- The warning is removed from the Warnings list.

### Create Warnings from Tag Limits
Warnings could be created automatically by entering tag limits min and/or max with selected checkboxes **Create Warning**. Follow the steps [Create warnings from tag limits.](/admin/data/#create-events-and-warnings-from-tag-limits)

For example: Select machine M45 and tag 27.Override feed. Enter Min=40and Max=80 with checked Create warnings.

- There are created two warnings and 4 events. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.103.png)

*Figure 101: Upkip Administration - Warnings of type Alarm*

After creating warnings their type could be edited from drop down and changed to Information, Warning or Alarm.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.104.png)

*Figure 102: Upkip Administration - Edit warning - change severity*

Trigger the warning by submitting value by IoTHub Tester to tag that is outside and entered min-max limits. For example submit telemetry.json

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.105.png)

*Figure 103: Upkip Administration -Triggering warning by IoT Hub Tester*

- The warning is triggered and alarm is created.

#### Visualizing alarms on dashboards
The warnings of type **Alarms, Warnings or Information** could be visualized on dashboard panel.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.106.png)

*Figure 104: Upkip Visualization -Active warnings on dashboard*

#### Closing alarms and removing warnings from the list
Submit by IoTHub Tester value that trigger stop event for the warning. 

For example: for machine M45 and tag 27.Override feed with limits Min=40and Max=80, submit value 90 and it will stop the warning. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.107.png)

*Figure 105: Upkip Visualization -Active warnings - removed closed warnings*

The alarm is removed from the system warnings list

