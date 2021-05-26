---
title: "Persister Servers"
date: 2021-05-20T15:51:19+03:00
draft: false
weight: 24
---

**Purpose:** Persister servers are in the cloud platform. **Persister servers** are configured in Microsoft Azure as **Function App**. They get the information from Azure IoT Hub and transfer it to the Influx DB or Configuration DB.

Precondition: Log in Upkip Administration with Microsoft user. Select **Servers**.

Select menu **Persister servers.**

- There is opened form with list of **Persister Servers**.   

![](/images/Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.001.png)

*Figure 154: Upkip Administration - Persister servers*


Select in azure portal **All services>Function App**

- There are listed all function app applications

Filter by ‘persister’ and the list is filtered only with functional app for persister server.
![](/images/Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.002.png)

*Figure 155: Upkip Persister servers as Azure Function App*

There are developed the following function app as Persister servers:

- Persister Server Heartbeat
- Persister Server Integration
- Persister Server Telemetry
- Persister Server Telemetry Failed

