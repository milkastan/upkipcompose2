---
title: "Notification channels allowed time interval"
date: 2021-05-20T15:45:50+03:00
draft: false
weight: 18
---

**Purpose**: Configuration of allowed time interval for notifications for the user allows to disable receiving notifications by Viber, Email or SMS for time outside of the defined allowed time interval.

**Precondition:** User with role administrator is logged in Upkip Administration.
### Configure Notification channels for user with allowed time interval
Open users list by clicking on the users icon.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.143.png)

*Figure 141: Upkip Administration - Open users list*

From the users list select the user and click **Edit**. 

- Form for editing user is opened

`       `![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.144.png)

*Figure 142: Upkip Administration - Configure user with allowed time interval for notifications*

-  **Enter user email** for receiving email notifications. **Enter user phone number with area code** for receiving SMS or Viber messages.
-  **Select time zone** – e.g. (UTC+02:00)E.EUROPE STANDARD TIME
-  Select from drop down (EMAIL, SMS or Viber) 
-  Specify for each selected notification channel time From-To for allowed time interval
-  Click OK to save the user
- The user data are saved with entered times for each notification channel.

### Configure Notifications to Email, SMS, Viber
Configure events and notification to user email following the steps [Configure Event and Notification to User Email.](/docs/data/notifemails/#configure-event-and-notification-to-user-email) 

Configure events and notification to user phone by SMS following the steps [Configure Event and Notification to User phone by SMS](/docs/data/notifemails/#configure-event-and-notification-to-user-email)

Configure event and notification to Upkip Viber Notifier following the steps [Configure Notification to Viber](/docs/data/notifviber/#configure-event-and-notification-to-viber) and [Subscribe to Upkip Viber Notifier](/docs/data/notifviber/#subscribe-to-upkip-viber-notifier)

### Submit Notifications within or outside of the allowed time interval
Submit notification to user email following the steps [Submit Notification to User Email.](/docs/data/notifemails/#submit-notification-to-user-email)

Submit notification to user phone by SMS following the steps [Submit Notification to User Phone by SMS](/docs/data/notifsms/#submit-notification-by-sms)

Submit notification to user phone by Viber Upkip Notifier following the steps [Submit Viber Notification.](/docs/data/notifviber/#submit-viber-notification)

Trigger the event and notification for each notification channel during the specified time interval. 

- The **notification is sent.**

Trigger the event and notification for each notification channel outside the specified time interval.

- The **notification is not sent**.


