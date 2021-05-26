---
title: "Organization structure"
date: 2021-05-20T15:42:33+03:00
draft: false
weight: 6
---

**Purpose:** Organization functionality in Upkip Administration allows to create hierarchical structure of the factory with base units – **Factory, Department and Machine.** Machines are defined with their **properties, tags and alarms**. Machine can be added to factory layout floors selecting visualization model. Machine models can be moved, resized and arranged on the factory floors. Created layout design with factory machines is shown in the Upkip Visualization application.

### **Add Factory**
**Purpose**: By selecting menu **Organization** user can add the main unit in the organization **Factory**.

Precondition: User is logged in Upkip Administration by Microsoft account. 

Select the left menu **Organization**

- The tree for organization structure is opened. 

Click on **Add** button.

- There is allowed to add only **Factory**.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.016.png)

*Figure 15: Upkip Administration - Add Factory*

When selecting menu **Add/Factory** is opened form Properties. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.017.png)

*Figure 16: Upkip Administration - Add Factory properties*

Enter or select the following data:

- **Factory name**
- **Select group**, created in AAD related to the whole factory.
- Select **time zone**

Click **Add**. 

- The main element of organization tree is created.
### **Add Department**
Precondition: The main element in organization tree is added – Factory. Select the created factory in the organization tree. Then is possible only to add department. 

**Purpose**: There is possible to create different departments corresponding to factory structure.  Departments are connected with user groups in Azure Active Directory (AAD). Users added to this azure group can see only machines from this department.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.018.png)

*Figure 17: Upkip Administration - Add Department under Factory*

When selecting **Add/Department** is opened form for new department. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.019.png)

*Figure 18: Upkip Administration - New department properties*

1) Enter **Department name**
1) Select **Group** from drop down (Groups are created in AAD)
1) Click **Add**
   - The created department is added under node **Factory**.

### **Add Machine**
Precondition: The main element in organization tree is added – Factory. Under the Factory are added Departments. Select some department to add Sensor (Machine). 

**Purpose:** There is possible to add under departments different sensors or machines by selecting **Add/Sensor.**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.020.png)

*Figure 19: Upkip Administration - Add Sensor under department*

- The form for entering machine data is opened. 

Fill in the form the following data:

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.021.png)

*Figure 20: Upkip Administration - New machine properties*

- **Name** – machine or sensor name e.g. M1 - Nakamura WT-300. It is good to contain sensor id.
- **Active Status 	-** the active machine status, e.g. ACTIVE
- **Active Status Clears Alarms** – checkbox  
- **Downtime Allowed Delay Seconds –** e.g. enter the number of seconds – 60.
- **Downtime Allowed Delay Status** – e.g. IDLE
- **Downtime Working Status** – for example: “ACTIVE,MACHINE OFFLINE,SYSTEM OFFLINE,MACHINE ONLINE,SYSTEM ONLINE”
- **Has Part Counter** – checkbox
- **Is Simulated** – checkbox
- **Model ID** – There are different visualization models. Selected model is visualized at the right. This model will be shown on Factory Layout 3D design. Some models are animated.
- **Sensor ID**	- sensor id has to be unique for the organization
- **Team** – select from drop down the configured teams in the factory.
- **Type ID**-  select from drop down the sensor type. The supported sensor types are: Fanuc, Mazak, Heidenhain, Datron, OPC UA, OPC Classic, OPC UA, Fanuc Robot, Facility, Deburring cell, UR Nakamura Cell, Robotic Cell
- **Whitelisted Alarms –** e.g. NONE,UNAVAILABLE,MAGAZINE IS RUNNING; Normal

Click **Add** button

- Machine (Sensor) is added under department
- Machine tags are automatically loaded depending on the machine type (Type ID). To view different machine types properties and tags go to [Machine Types](#_Machine_Types)


![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.022.png)

*Figure 21: Upkip Administration - Configured machine under department*