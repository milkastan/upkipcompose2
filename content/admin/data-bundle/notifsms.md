---
title: "Notifications by SMS"
date: 2021-05-20T15:45:50+03:00
draft: false
weight: 16
layout: redirect
---

**Purpose**: Notifications could be configured to submit messages to **user phone by SMS.** Notifications are triggered by Event. In the Event is defined expression on some machine or sensor tag. If the event has occurred then notification is triggered and defined message in the notification is submitted to user mobile phone as SMS. 

### Configure User in Upkip Administration
[Configure Users in Upkip](/admin/users/#usersgroups)

### Configure Notification by SMS
Select the machine (or sensor) ID and tag which will be used in Event configuration.

Select the machine tag by following the steps in [select machine or sensor Tag](/docs/data/notifteams/#configure-event-and-notification-to-teams)

To create event see [Create event manually](/admin/data/#create-events-manually)

Select menu **Notifications.** 

- The list of notifications for the organization is shown with name, subject and text.
-  Click **New** button to create new notification

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.142.png)

*Figure 140: Upkip Administration - Create notification with media type SMS*

Enter to create notification:

-  Name, Message subject, Message text. 
   -  Message subject
   -  Message text will be shown  as SMS text. There is possible to select some predefined placeholders by clicking on **+Placeholders** and select from the list.
-  Click to **Add** event. Select from the list created event in [Create event manually](/admin/data/#create-events-manually)
-  Click New to enter Address, Media Type and Address Type
   - For **Media Type** select **SMS**
   - For **Address Type** select **User**. 
   - For **Address**, click and select user from the list with users
-  Click **Save** to save the notification.

The Notification  will be saved in Notification list.

### Submit Notification by SMS
[Simulate event by IoT Hub Tester](/admin/data/#simulate-event-by-iot-hub-tester)

Submitted data to machine tag will trigger the related event. 

Notification to SMS with this event will be executed and submit SMS to user phone. 

Message Text from Notification will come as SMS text.

