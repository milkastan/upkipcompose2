---
title: "Machine Tags and Alarms"
date: 2021-05-20T15:43:19+03:00
draft: false
weight: 8
---

**Purpose**: Machine tags are used for receiving data from machine. Received data is analyzed and used for visualization in different dashboards presenting by user friendly view the received data from machines.

### Machine Tags
Precondition: Machine is selected in organization tree.  At the right select TAGS. 

- The list of configured tags for machine is opened.
- For each tag is shown: **ID, Name, Type, Payload, Display Name, Source**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.043.png)

*Figure 41: Upkip Administration - Machine tags*

**Source** of the tag indicates tag origin with specific icon before description:

- **Machine type** – the supported machine types are: **Fanuc, Mazak, Heidenhain, Datron, OPC UA, OPC Classic, Fanuc Robot, Deburring cell, UR Nakamura Cell, Robotic Cell.** 
- **System** - system tags are common tags for all machine types 
- **External sensors** - this appears for tags connected to external sensors. Supported type of external sensors are: **Disruptive technologies, ReMoni, El-Watch, Neuron sensors, NCD sensors, Weather data** etc. 

**Filtering machine tags** – machine tags can be filtered by typing in the filter field

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.044.png)

*Figure 42: Machine tags - Filtering the tags*

- Only tags containing in the name, payload, display name typed text are shown.

**Created alarms for tags** are indicated with icon in the first column after the Tag ID.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.045.png)

*Figure 43: Machine tags - icon for created alarms from tag*

### Edit Tag
Precondition: Machine is selected in organization tree.  At right select TAGS. 

- The list of configured tags for machine is opened.

Select some tag and click Edit.

- Form for editing tag is opened.

Tag with **value type String** has the following data:

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.046.png)

*Figure 44: Upkip Administration -Edit machine - Add new tag*

-  **Tag Name** – has to be unique
-  **Type** – value type – String (Int, Float, File)
-  **Description** – description of the tag
-  **Tag Type** - select from predefined
-  **External source** – selecting None or some external sensor if installed

**Tag of type INT or Float** has 3 additional fields – Min, Max and Set Point.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.047.png)

*Figure 45: Upkip Administration -Edit machine - Add new tag Min and Max limits*

`**Min** and **Max** fields are used to enter integers/floats for minimal and maximal value.

**Set Point** is used to enter the optimal value as integer/float.

Min and/or Max values can be used for create warnings for them following the steps 


### **Add Tag**
Precondition: Machine is selected in organization. Select tab TAGS.

- List of machine tags is shown

To add new tag click **New button** and select **menu Tag**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.048.png)

*Figure 46: Machine - Tags - Add new tag*

- Form for adding new tag is opened

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.049.png)

*Figure 47: Machine - Tags - Add new tag*

When adding new tag user has to fill in data in the same fields as in [Edit Tag.](#edit-tag) 

### Add Tag with External sensor
Precondition: Machine is selected in organization. Select tab TAGS.

- List of machine tags is shown

The external sensors can be connected to:

- **Machine** tags to measure different temperatures related to machine: coolant, motor, body, spindle, cooling pump etc., vibration and power.
- **Rooms** tags to measure temperature, door sensor, weather etc.

Data received from external sensors are visualized as charts showing min, max, average values and current values.

Upkip supports external sensors of the following types:

- **ReMoni** 
- **Distuptive Technilogies**
- **El-Watch** - the old one of Neuron sensors
- **Neuron sensors**  -the new one of Neuron sensors
- **NCD** **sensors**
- **Weather**

How to install external sensors is described in document “Integration- External Sensors.docx”

To configure external sensors open menu **Organization.** Find machine under departments and select. Open Tags. Find the tag connected with external sensor by filtering.

- Tag connected to external sensor is filtered.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.050.png)

*Figure 48: Upkip Administration -External sensors connected to machine tags*

Select tag and click **Edit**

- Form for editing tag with external sensor is opened

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.051.png)

*Figure 49: Upkip Administration -Edit machine tag with connected external sensor*

In addition to fields described in [Add Tag](#_Add_Tag_-  tags connected to external sensors have attributes:

-  **External Source** – selected external source from the list of supported types – ReMoni, Disruptive Technologies, El-Wawtch, Azure ML LC, Weather, Neuron Sensors, NCD Sensors.
-  **External type –** Data or Alarm. When select Data additional fields are shown. 

When adding tag connected to external sensor expand the drop down **External source** and select type of the sensors. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.052.png)

*Figure 50: Add tag - Select external sensor type*

When selecting type of the external sensors additional fields are shown for configuration. 

External sensors of type **ReMoni** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.053.png)

*Figure 51: Add tag - external sensor ReMoni configuration*

After selecting type of external sensor, fill in base URL with username and password.

Select external type – **Data or Alarm**. When Data is selected additional fields for sensor id, channel number and data type have to be filled in. 

External sensors of type **Disruptive technologies** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.054.png)

*Figure 52: Add Tag - external sensor Disruptive technologies configuration*

External sensors of type **El-Watch** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.055.png)

*Figure 53: Add Tag - external sensor El-Watch configuration*

External sensors of type **Neuron sensors** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.056.png)

*Figure 54: Add Tag - external sensor Neuron sensors configuration*

External sensors of type **NCD PPMS sensors** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.057.png)

*Figure 55: Add Tag - external sensor NCD PPMS sensors configuration*

External sensors of type **NCD PMS sensors** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.058.png)

*Figure 56: Add Tag - external sensor NCD PMS sensors configuration*

External sensors of type **Weather** configuration: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.059.png)

*Figure 57: Add Tag - external sensor Weather configuration*

### **Import tags from file**	

Tags for machine could be imported from **CSV**. Select tab **+Provision** for machine. TAB is visible only for users with role system administrator.

Upload CSV file with description for each tag: name, valueType, (PayloadType),(DisplayName)

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.060.png)

*Figure 58: Upkip Administration -Edit machine - Import tags*

### Delete Tag
Precondition: Machine is selected in organization tree.  TAGS tab is selected at the right. 

- The list of configured tags for machine is opened.

Select some tag and click Delete. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.061.png)

*Figure 59: Tags - Delete tag confirmation*

- Tag is deleted. If  tag has created events they also are deleted. 

### Preview and manage tags
Precondition: Machine is selected in organization tree.  TAGS tab is selected at the right. Click on **Preview Data** button.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.062.png)

*Figure 60: Tags list - Open Preview Data*

- Preview Data form is opened with interval **Date From – Date To** loaded by default one moth back. Filter Selecting tags is **All** by default. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.063.png)

*Figure 61: Preview Tags form*

**Purpose**: Preview and manage tags form allows for a user system administrator to:

- View and filter tags for the selected time period
- View tags data as last value, min, max, avg and count for the selected time period
- View if tags has events or calculated tags
- View tags source (system, machine type or external sensors)
- Some tags is possible to select and disable. Tags are marked in the DB and are hidden from the list
- Disabled tags is possible to delete permanently

Clicking on the **Search** button the form is loaded with all machine tags with their data for the selected time period.  

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.064.png)

*Figure 62: Tags - Preview Data*

Tags are shown in the table with:

- Name and Display Name.
- Last - last value and Count - values count for the selected time period
- For tags of type integer are shown: Min, Max, Average values for the selected time period;
- The number of events and calculated tags in which they participate
- Source – tag source. 

**Source** of the tag** indicates tag origin with specific icon before description:

- **Machine type** – the supported machine types are: Fanuc, Mazak, Heidenhain, Datron, OPC UA, OPC Classic, Fanuc Robot,  Deburring cell, UR Nakamura Cell, Robotic Cell
- **System –** system tags are common tags for all machine types – see 
- **External sensors –** this appears for tags connected to external sensors. Supported type of external sensors are: Disruptive technologies, ReMoni, Neuron sensors, Weather data etc.  see [Add Tag with external sensor](#add-tag-with-external-sensor)

**Filtering the tags** is possible by the following options: **All, Empty tags, Tags with data, Disabled tags**. Filtering the tags is possible also by typing in the filter field.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.065.png)

*Figure 63: Preview Data - filtering tags*

Filtering by **Empty tags** – there are shown only tags without any data for the selected time period. 

When selecting **Tags with data** – in the form are listed only tags with data for the selected time period.  

Some tags is possible to select by checkboxes and disable by clicking **Disable tags** button. 

- Disable confirmation form is opened. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.066.png)

*Figure 64: Preview Tags - Disable tags confirmation*

If filter tags with Disabled tags from the filter is shown list of disabled tags. At the bottom are visible buttons **Delete tags** and **Close**. If select tags that do not have events or calculated tags is shown confirmation popup. It clicking Delete button the tag is deleted. There are possible to select many tags and delete. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.067.png)

*Figure 65: Preview Tags - Delete tag confirmation*

If tag or tags have events of calculated tags in the confirmation warning are listed events or calculated tags with selected tag and is offered to replace tag in events or calculated tag with another tag. After selecting another tag is possible to delete selected tag.

- Tag in events and calculated tag is replaced with selected tag.
- Tag is deleted from machine.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.068.png)

*Figure 66: Preview Data - select tag to replace and delete tag*

### Machine Alarms
Edit selected machine from organization tree. Select tab Alarms

- There are configured all alarms messages for machine

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.069.png)

*Figure 67: Upkip Administration - Edit machine - Machine alarms messages*

There is possible to create automatically notifications from alarms by selecting alarms and pressing button Create Notification. Follow the steps in [Notifications from machine alarms](#notifalarms). 

Created notifications from alarms are indicated with notification icon in the first column.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.070.png)

*Figure 68: Machine Alarms - indication for alarms with notifications*