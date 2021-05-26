---
title: "Gateways"
date: 2021-05-20T15:43:19+03:00
draft: false
weight: 9
---

**Purpose**:  Gateways are configured in Microsoft Azure as **IoT Devices** or **IoT Edge devices** and are installed on the computers in the manufacturer premises. 

They acts as a **Cloud Gateway** which:

- **Connects** with on-premises hardware;
- Reads, transforms and buffers **data by different adapter modules;**
- Interacts with the **Azure Cloud** infrastructure to send data and receive configurations;
- Is set with **Recovery** settings to Restart 15 minutes after each failure;

Precondition: Log in Upkip Administration with Microsoft user. Select **Organization**.

Select menu **Gateways**.

- There is opened form with list of **Gateways**. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.147.png)

*Figure 145: Upkip Administration - Gateways*

For example, in the Upkip Administration are used the following gateways (IoT devices or IoT Edge devices)

- **Used by the system internally:**
- **Calculated Tags** (DeviceId: CalculatedTagAnalyser)
- **ExternalTelemetry** (DeviceID: ExternalTelemetryProcessor)
- **Warnings** (DeviceID: EventProcessor)
- **Health Check** (DeviceID: HealthCheckTestSensor)
- **Synchronizer** (DeviceID: RefreshTimer)
- **Software gateways installed on premises:**
- **Windows** (Developed by ICB as a windows service)
- **Linux (Edge)** (Developed by ICB as Azure IoT Edge device)


In the **Gateway/Properties** are defined properties of gateway: **Name, Device ID, Desired and Reported configurations**. By clicking on button **Edit Json** is possible to edit gateway configuration written as json data. Reported configuration is returned by azure and is usually equal to desired configuration. 

When selecting in Upkip Administration **Gateways>Windows>Modules** are listed the modules: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.148.png)

*Figure 146: Upkip Administration - Gateway modules*

In the **Microsoft Azure>IoT Hub>IoT devices** the following devices are created automatically: 

- **EventProcessor, RefreshTimer, ExternalTelemetryProcessor, EventProcessor, CalculatedTagAnalyser.**

The modules are run on the configured IoT devices. 

For example: On the IoT device **DUBUG-WS378-Win** run the modules for different adapters: ABBRobotAdapter, BalluffAdapter, ExcelAdapter, FanucFocasAdapter, FanucRobotInterfaceAdapter, FanucRobot-Mazak218, M45-Heidenhain, MTCAgentAdapter, MTCCollectorAdapter, SiemensS7Adapter, SQLAdapter, ExcelAdapter.

Clicking on the configured device in azure are listed the modules running on it.   

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.149.png)         ![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.150.png)

*Figure 147: IoT Hub - IoT Devices                                   Figure 148: IoT Hub - IoT Device Modules*

When selecting in Upkip Administration **Gateways>Linux (Edge) >Modules** are listed the modules: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.151.png)

*Figure 149: Upkip Administration - Gateways - Linux modules*

Gateway Linux (Edge) is configured on **Azure>IoT Hub>IoT Edge device**. Clicking on some IoT Edge device are listed modules that run on the device. For example: When clicking on the IoT Edge device ‘DEBUG-WS378’ are listed the modules:

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.152.png)                                ![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.153.png)

*Figure 150: IoT Hub - Linux IoT Edge devices                                   Figure 151: IoT Hub - IoT Edge Device modules*