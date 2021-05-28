---
title: "Notifications to User Emails"
date: 2021-05-20T15:45:23+03:00
draft: false
weight: 14
layout: redirect
---

**Purpose**: Notifications could be configured to submit messages to **user email.** Notifications are triggered by Event. In the Event is defined expression on some machine or sensor tag. If the event has occurred then notification is triggered and defined message in the notification is submitted to user email. 

### Configure User in Upkip Administration
Users in Upkip Administration are configure following the steps [Users Management](/admin/users/#usersgroups)

Log as user with role System Administrator in Upkip Administration. 

Find in **Users list** the user and click **Edit**. Make sure that **user email** **is configured** in E-Mail field. This is the email to which will be sent email notification. This email could be different from username email.

- In the user details is entered phone number with area code

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.139.png)

*Figure 137: Upkip Administration - User configuration with email*

### Configure Event and Notification to User Email
Select the machine (or sensor) ID and tag which will be used in Event configuration.

Select the machine tag by following the steps in [Search and add Tag](/admin/data/#search-and-add-tag)

To create event see [Create event manually](/admin/data/#create-events-manually)

Select menu **Notifications.** 

- The list of notifications for the organization is shown with name, subject and text.
Click **New** button to create new notification

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.140.png)

*Figure 138: Upkip Administration - Create notification with media type email*

Enter to create notification:

-  Name, Message subject, Message text. 
   -  Message subject will appears as Email Subject
   -  Message text will be shown  as email text of the message. There is possible to select some predefined placeholders by clicking on **+Placeholders** and select from the list.
-  Click to **Add** event. Select from the list created event in [Create event manually](/admin/data/#create-events-manually)

-  Click New to enter Address, Media Type and Address Type
   - For **Media Type** select **Email**
   - For **Address Type** select **User**. 
   - For **Address**, click and select user from the list with users
-  Click **Save** to save the notification.

The Notification  will be saved in Notification list.

### Submit Notification to User Email
[Simulate event by IoT Hub Tester](/admin/data/#simulate-event-by-iot-hub-tester)

Submitted data to machine tag will trigger the related event. 

Notification to email with this event will be executed and submit email to user email. 

Email will be from a sender <noreply@i4sbased.com> (for test environment) with

- **Email Subject** equal to Notification **Message Subject**
- **Email message** text equal to Notification Message Text

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.141.png)

*Figure 139: Notification email with configured message text*

