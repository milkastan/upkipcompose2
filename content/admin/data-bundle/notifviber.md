---
title: "Notifications to user Viber"
date: 2021-05-20T15:45:37+03:00
draft: false
weight: 15			
layout: redirect
---

**Purpose**: Notifications could be configured to submit messages to **Viber public account**. Users subscribed to this account can receive message from configured Notifications. Notifications are triggered by Events. In the Event is defined expression on some machine or sensor tag. If the event has occurred then notification is triggered and defined message in the notification is submitted to Viber Upkip Notifier. 

### Configure User in Upkip Administration
Precondition: Users in Upkip Administration are configured following the steps [Configure Users in Upkip](/admin/users/#usersgroups)

Log as user with role System Administrator in Upkip Administration. 

Find in **Users list** the user and click **Edit**. Enter in the **Phone Number with Area code** the user **phone number** that will be used for Viber notification.

- In the user details is entered phone number with area code

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.133.png)

*Figure 131: Upkip Administration - User configuration with phone number*


### Configure Event and Notification to Viber
*Precondition:** User logged in Upkip Administration. Select organizationà Menus for selected organization are shown. 

Select the machine tag by following the steps in [Search and add Tag](/admin/data/#search-and-add-tag)

To create event see  [Create event manually](/admin/data/#create-events-manually)

Select menu **Notifications.** Click New à form for creating notification is opened.

Fill in the Notification form the data:

-  Notification name
-  Message subject
-  Message text. There is possible to use Placeholders from the list by clicking on **+Placeholders.**
-  Events – select created event from the events list
-  Addresses – select:
   -  Media Type – select **Viber**
   -  Address Type – select **User**
   -  Address - doubleclick and select our configured user with the phone for viber notifications. The selected user appears in the address field.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.134.png)

*Figure 132: Upkip Administration - Create notification with message to Viber phone number*

Click **Save**

- Notification with Media Type **Viber** is created.
- **Viber Invitation email** is sent to the user email. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.135.png)

*Figure 133: Upkip Viber invitation email*
### Subscribe to Upkip Viber Notifier
Precondition: User has received Viber invitation email. Invitation email contains QR code for Upkip Viber Notifier.

Scan QR Code with the mobile device and open the link or click the link bellow to gain access to Upkip Notifier Viber public account.

Click on the **Chats** button to open Viber chat.

Type on the chat and submit message with text

**.subscribe [email_address@example.net]**

- There appears response from Viber bot :“A verification email has been sent to your email address.”
- **Verification email is sent** to the user email with subject: Viber Verification and text:

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.137.png)

*Figure 135: Upkip Viber verification email*

Open the received email and click on the link **Verify** to make email verification.

- In the browser is opened page for successful verification.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.138.png)

*Figure 136: Upkip Viber Verification confirmation page*

- In Viber is received message from Viber Bot : “You are successfully subscribed with email **email_address@example.net**”

### Submit Viber Notification
Preconditions:
- User is subscribed successfully for Viber Upkip Notifier account
- Notification is configured with event, and Address= "user email", Media Type=Viber, Destination=User

Simulate the event with IoT Hub Tester to trigger the event and notification to Viber 

[Simulate event by IoT Hub Tester](/admin/data/#simulate-event-by-iot-hub-tester)

When some event is triggered, notification with Media Type=Viber and Destination=User has to submit message to user **Upkip Notifier Viber account.** 