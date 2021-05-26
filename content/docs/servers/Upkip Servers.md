### **Persister Servers**
`      `**Purpose:** Persister servers are in the cloud platform. **Persister servers** are configured in Microsoft Azure as **Function App**. They get the information from Azure IoT Hub and transfer it to the Influx DB or Configuration DB.

Precondition**:** Log in Upkip Administration with Microsoft user. Select **Organization**.

`       `Select menu **Persister servers.**

- There is opened form with list of **Persister Servers**.   

`    `![](Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.001.png)

*Figure  SEQ Figure \\* ARABIC 154: Upkip Administration - Persister servers*



Select in azure portal **All services>Function App**

- There are listed all function app applications

Filter by ‘persister’ and the list is filtered only with functional app for persister server.

`     `![](Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.002.png)

*Figure 155: Upkip Persister servers as Azure Function App*

There are developed the following function app as Persister servers:

- Persister Server Heartbeat
- Persister Server Integration
- Persister Server Telemetry
- Persister Server Telemetry Failed

### **Analysis Servers**
`      `**Purpose:** Analysis servers are in the cloud platform. **Analysis servers** are configured in Microsoft Azure as **Function App**. They take the information from Influx DB or Configuration DB and make different calculations (as OEE, utilization, etc.)

Precondition**:** Log in **Upkip Administration** with Microsoft user. Select **Organization**.

`       `Select menu **Analysis servers (1).**

- There is opened form with list of **Analysis Servers**.   Clicking on analysis server (2) is opened list of implemented Analysers (3). They are implemented in azure as Function App. 

![](Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.003.png)

*Figure 156: Upkip Administration - Analysis servers*

Select in the azure portal **All services>Function App (1)** and filter by analyser (2).

- There are listed all function app for different analysers (3)

There are developed the following Analysers:

- Alarm Analyzer
- Downtime Analyzer
- Data Summary Analyzer
- Service Health Analyzer
- OEE Analyzer
- Time series Context Analyzer
- Order Analyzer
- Report Analyzer
- Machine KPI Analyzer
- Calculated Tags Analyzer

![](Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.004.png)

*Figure 157: Upkip Analysers as Azure Function App*


### **Notification Servers**
**Purpose:** Notification servers get and information from Influx BD or Configuration DB and analyze it.  If some event is triggered and there is configured notification with it, the notifications are sent to configured user or destination. There are supported notifications to user email, user viber, user phone as SMS and Microsoft Teams.

Precondition**:** Log in **Upkip Administration** with Microsoft user. Select **Organization**.

`       `Select menu **Notification servers (1).**

- There is opened form with list with **Notification Servers**

`        `**![](Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.003.png)**

*Figure 158: Upkip Administration - Notification servers*
**
`        `Notification server and Event Processor are implemented in Azure as Function App.

`     `Select in the azure portal **All services>Function App (1)** and filter by event or notification (2).

- There are listed function apps for notification server or Event processor.
**
`    `The following Function App are developed as Notification servers:

- Event processor
- Notification server

![](Aspose.Words.0026e4dc-4cb1-409d-91ad-eda9ac21484a.005.png)

*Figure 159: Upkip Notification servers as Azure Function App*




