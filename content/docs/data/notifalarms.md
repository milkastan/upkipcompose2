---
title: "Notifications from machine alarms"
date: 2021-05-20T15:44:37+03:00
draft: false
weight: 13
---


**Purpose**: There is possible in Upkip Administration, selecting some machine, from the machine alarms list to click  some alarm(s) and Create Notification by email.

**Precondition**: User with role Administrator is logged in Upkip Administration
### **Create Notification by selecting machine alarm**
Select menu **ORGANIZATION**. In the organization tree find the department and select machine. 

- At the right side for the selected machine are visible tabs **PROPERTIES, TAGS, ALARMS, +PROVISION**

Click on **ALARMS** 

- The list of machine alarms is shown

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.145.png)

*Figure 143: Upkip Administration - Create notification by selecting machine alarm message*
### **Submit created notification from machine alarm**
Find by the filter some alarm (s), **select them by the checkbox** 

Click on the button **Create Notification**. 

- Automatically are created **Event and Email Notification for selected alarms**
- The form **Edit Notification** is opened automatically filled

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.146.png)

*Figure 144: Upkip Administration - Edit notification automatically opened*

The created automatically notification which is prefilled could be edited and saved.

-  **Name:** **Sensor ID Alarm Notification <current date and time>**.
-  **Message Subject: Sensor ID Alarm Occurred**. 
-  **Message Text**: Filled with place holders {EVENTTIME}: "{TAGVALUE}". There is possible to add additional text or insert placeholders from predefined.
-  **Events**: Automatically is selected created Event for selected alarm. 
-  **Addresses**: Automatically are added MediaType=Email, AddressType=User and Address=email of the user logged in administration. Email of the user can be changed by selecting from the list.

If alarm message is sent to machine tag of type Alarm, the event is triggered. 

Notification email configured with it also is executed (For example submitted email to user).
