---
title: "Notifications to Microsoft Teams"
date: 2021-05-20T15:46:24+03:00
draft: false
weight: 17
layout: redirect
---

**Purpose**: Notifications could be configured to submit messages to **Microsoft Teams channel** where invited to Team peoples can read them and reply. Notifications are triggered by Event. In the Event is defined expression on some machine or sensor tag. If the event has occurred then notification is triggered and defined message in the notification is submitted to configured teams channel. To work notifications to Teams, the member <Upkip.Notifier@icb.bg> has to be added to the Team.

#### Microsoft Teams Configuration
The user should be owner or invited to some Team in Microsoft Teams. 

The user has opened **Microsoft Teams** and view created Teams and channels

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.118.png)

*Figure 116: Microsoft Teams Configuration*

After creating some Team default channel **General** has created. 

Additional channel can be added to the team.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.119.png)

*Figure 117: Microsoft Teams Configuration - Add channel*

Right click on the **Team menu** and select **Manage Team**

- Manage Team page is opened with selected menu **Members**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.120.png)

*Figure 118: Microsoft Teams Configuration - Manage Team*

Type in the member search field – Upkip Notifier. If the member not added to the team click **Add member** and type **Upkip.Notifier@icb.bg** and add to the team. 

- Upkip Notifier must be added to the Team (This member is used only for system purposes)

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.121.png)

*Figure 119: Microsoft Teams Configuration -Manage Team - Add member Upkip Notifier*

Get the channel link by right click on the channel menu and select **Get link to channel.**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.122.png)

*Figure 120: Microsoft Teams Configuration - Channel - Get link to channel*

Copy the link to clipboard by clicking on **Copy** button

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.123.png)

*Figure 121: Microsoft Teams Configuration -Copy link to channel*

- The link to channel is copied to clipboard and will be used to configure Notification in upkip Administration.
#### Configure Event and Notification to Teams 
Precondition: Log in the Upkip Administration using credentials for different environment described in document I4SME Environment Configuration.docx

Select **organization** for which will be configured events, notifications and messages submitted to the Microsoft Teams.


##### Select Machine or Sensor Tag
Select menu **Organization** and expand the **organization tree**. Find the machine, its sensor ID and Tag, for which will be created Event.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.124.png)

*Figure 122: Upkip Administration - Get machine ID*

**Sensor ID** will be used when simulating and submitting telemetry for the machine tag.

Click on the tab TAGS and select machine TAG. Tag **Name and Payload** are important when submitting and simulating telemetry for the machine and tag

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.125.png)

*Figure 123: Upkip Administration - Get machine tag payload*

##### Configure Event for the selected Tag
Select menu **Events**. 

- The  events for the organization are listed in the table. Each event has Name and Expression.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.126.png)

*Figure 124: Upkip Administration - Create event with expression*

Create new event for selected tag name (e.g. 6.Availability). Click on the **New** button, enter event name, enter expression (e.g. lastValue('6.Availability')=’STOPPED’) and click **Save**.

- The new event with name and expression is created. It will be used for our notifications to Microsoft Teams.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.127.png)

*Figure 125: Upkip Administration - Created event in events list*

##### Configure Notification with created Event
Select menu **Notifications.** 

- The list of notifications for the organization is shown with name, subject and text.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.128.png)

*Figure 126: Upkip Administration - Create notification with destination Teams*

-  Click **New** button to create new notification

Enter to create notification:

-  **Name, Message subject, Message text.** Message text will be shown in Microsoft team channel. There is possible to select some predefined placeholders by clicking on **+Placeholders** and select from the list.
-  Click to **Add** event. Select from the list created event.
-  Click **New** to enter **Address, Media Type and Address Type**
   -  In the address, paste the copied **channel link**
   -  For Media Type select **MicrosoftTeams**
   -  For Address Type select **Destination**. 
-  Click **Save** to save the notification.

The created Notification will appears in the Notifications list.

#### Simulate event by IoT Hub Tester

**Configure Azure IoT Hub Tester** in the selected environment. The application will be used to submit telemetry to the selected machine tag with data that will be trigger the created event and then notification. The message text in the notification will be submitted to Microsoft team channel.

**Prepare Telemetry json**
![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.129.png)

*Figure 127: IoTHub Tester - simulate submitting value to machine tag*

**IoT Hub Tester** is connected to Azure Environment and created device.

**Submit Telemetry json**
Important data in the Telemetry.json are: **Sensor ID, Payload Type and Payload Data,** submitted to machine tag. Timestamp could be changed. 

**View submitted data in Upkip Visualization**
In the document Telemetry DataFlow.docx, in the topic Visualize Data, is described how to view in created dashboard submitted data for tag. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.130.png)

*Figure 128: Upkip Visualization - View submitted data on test dashboard*

If simulated data are visible in visualization application, event and notification are configured properly, the message from notification should be listed in the Microsoft Team channel. 

- When submitting values for sensor ID, Payload type, and  values, they are visible in the table.

#### Submit Messages to Microsoft Teams
Open Microsoft Teams and select created channel for notifications. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.131.png)

*Figure 129: Microsoft Teams - View submitted message from notification*

When event and notification are triggered, the message is submitted to Teams and will be visible from all members of the team.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.132.png)

*Figure 130: Microsoft Teams - Reply to Upkip Notifier message*

The members of the Team can click Reply, notify someone about the message by typing ‘@’ before their name. 
