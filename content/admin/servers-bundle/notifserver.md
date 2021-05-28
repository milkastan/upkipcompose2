---
title: "Notification Server"
date: 2021-05-20T15:51:19+03:00
draft: false
weight: 26
layout: redirect
---

**Purpose:** Notification servers get and information from Influx BD or Configuration DB and analyze it.  If some event is triggered and there is configured notification with it, the notifications are sent to configured user or destination. There are supported notifications to user email, user viber, user phone as SMS and Microsoft Teams.

Precondition: Log in **Upkip Administration** with Microsoft user. Select **Organization**.

Select menu **Notification servers.**

- There is opened form with list with **Notification Servers**

![](/images/Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.003.png)

*Figure 158: Upkip Administration - Notification servers*

Notification server and Event Processor are implemented in Azure as Function App.

Select in the azure portal **All services>Function App (1)** and filter by event or notification.

- There are listed function apps for notification server or Event processor.
**
The following Function App are developed as Notification servers:

- Event processor
- Notification server

![](/images/Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.005.png)

*Figure 159: Upkip Notification servers as Azure Function App*
