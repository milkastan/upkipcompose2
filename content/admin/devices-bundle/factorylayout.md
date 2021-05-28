---
title: "Factory layout"
date: 2021-05-20T15:43:19+03:00
draft: false
weight: 7
layout: redirect
---

## Configure Factory Floors
Precondition: User has logged in Upkip Administration. Organization menu is selected.

User clicked on configuration icon on top right of organization tree

- At the right are shown tab **Configure** (and Factory layout if already configured)

**Purpose**: The form is used to define main properties and upload the pictures for the factory floors.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.023.png)

*Figure 22: Upkip Administration - Configure factory layout and floors*

User can define:

- **Map width and height** – size of the area where the factory layout will be designed
- Background color, text font size, new machine color, new machine size and opacity
- By **Add Floor** user can add floors for factory layout (up to three)
- For each floor is possible to upload pictures on which to show the machines

To upload pictures for the factory floors: 

- Add floor by **clicking Add Floor (1)**
  - The row for uploading picture for floor is added
- By clicking on **upload button (2)** select some picture from the local disks and upload
  - The floor picture is uploaded on azure
- User can remove uploaded picture by **Delete** button. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.024.png)

*Figure 23: Configure factory floors*
### Add machine to Factory Floor
Precondition: Machine is added in organization tree. 

**Purpose**: Selected machine can be added to some of defined floors of the enterprise. 

` `![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.025.png)

*Figure 24: Add machine to factory floor*

Select machine in organization tree. Click button **Add to floor** and select from menu one of the configured floors.

- Machine is added to the selected floor. 
- Machine appears at the center of the selected factory floor. 
- Machine Data form appears at the right side.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.026.png)

*Figure 25: Organization - Add machine to floor*

### Connect animation with machine statuses

When machine is added to the floor and selected at the right appears **Machine Data.** Machine models is possible to develop with some animation. 

`    `![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.027.png)

*Figure 26: Selected machine on the floor – Animations*

In the section Animations is possible to select machine status to connect it with animation. 

This means on the Factory Layout when machine has selected status the machine animation will be played. 

There is possible to **collapse and expand the main menu.** 

Collapsing the main menu increases the floor design area and shows all main menus only with icons.

Expanding the main menu shows all menus with icon and text. 

`  `![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.028.png)                                                  ![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.029.png)                        

*Figure 27: Upkip Administration -collapse main menu          Figure 28: Upkip Administration - expand main menu*


### Actions with machine
#### Select machine on the organization tree/floor
Precondition: Organization tree with departments and machines is created. Machine is added to the factory floor.

When selecting machine in the organization tree:

- If machine is added on some factory floor 
  - Floor map is shown with selected machine. 
  - Buttons **Floor, Properties, Tags, Alarms** are visible

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.030.png)

*Figure 29: Select machine from the tree - show machine selected on the floor*

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.031.png)

*Figure 30: Select machine from the tree - shows machine properties*

- If machine is not added to some factory floor
- At the right are shown buttons **Properties, Tags, Alarms**
- It appears under the tree button **Add to floor**. Clicking on the button **Add to floor** and selecting floor from menu, machine is added on the factory layout floor. Then machine can be arranged on the floor –  [Actions with machine](#_Actions_with_machine)

In reverse when selecting some machine in the factory layout floor, machine appears selected in the organization tree. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.032.png)

*Figure 31: Select machine on the floor - show machine selected on the organization tree
#### Move machine on the floor layout
Precondition: Click machine on the floor layout.

- Machine is selected with circle around it. 

Clicking on the machine without releasing the mouse is possible to move the machine to another location on the floor area.

` `On **Machine Data** form X and Y positions are changed. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.033.png)

*Figure 32: Factory floor - move machine on the floor layout*

Pressing **Save** button will save the floor with last machine location.
#### Resize and rotate machine on the floor layout
Precondition: Click machine on the floor layout.

- Machine is selected with circle around it. 

Machine models can be **resized and rotated.** 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.034.png)

*Figure 33: Machine model - resize or rotate*

By clicking on (1) machine can be resized, by clicking on (2) machine can be rotated on the map. 

When machines are located on their places on the floor map click button **Save** to save the created floor with machines locations.
#### Change machine floor
Precondition: Click machine on the floor layout.

- Machine is selected with circle around it (1)

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.035.png)

*Figure 34: Factory Design layout - move machine to other floor*

From **Machine Data** change current floor from drop down.

- Machine is moved on the selected floor.
- The new floor is opened with machine added in the center of the floor. 
- Arrange the machine location and save the layout.

#### Deselect machine on the floor layout
Precondition: Machine is selected on the floor layout.

- Machine appears selected also in the organization tree

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.036.png)

*Figure 35: Factory design layout - selected machine in the tree and on the floor*

Deselecting machine is possible by **clicking again on the selected machine.**

- Machine selection in the organization tree is removed 
- Organization tree is not collapsed
- At the main area are visible tabs: **Configure, Ground floor** (Floor1, Floor2 if configured)

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.037.png)

*Figure 36: Factory design layout - deselect machine by clicking on the selected machine*

Deselecting machine is also possible also by clicking **Refresh button** at the top right of the organization tree.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.038.png)

*Figure 37: Organization tree and layout - deselect machine by refresh*

After clicking the Refresh button

- Machine selection in the organization tree is removed 
- Organization tree is collapsed
- At the main area are visible tabs: **Configure, Ground floor** (Floor1, Floor2 if configured)
#### View machine properties
Precondition: Machine is configured in organization tree.

Selecting different machines on organization tree at the right are shown tabs **Floor** (if machine is added to the floor layout), **Properties, Tabs, Alarms**. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.039.png)

*Figure 38: Machine added to floor - tabs Floor, Properties, Tags, Alarms*

Selecting tab **Properties** are visible machine properties. Selected model is visualized at the right.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.040.png)

*Figure 39: Machine Properties with visualization model selected*

For different machine types are configured different properties. To see machine properties go to [Machine Types](#_Machine_Types). For each machine type are shown configuration of the properties.
#### View machine alarms
Precondition: Machine is configured in organization tree.

Select machine in organization tree. Select at the right tab **Alarms**. 

- If machine has alarms the list of machine alarms is shown. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.041.png)

Selecting some alarm (or alarms) is possible automatically to create event, alarm and notification for these alarms. Go to [Notifications from machine alarms](#_Notifications_from_machine). 

There is indication with icon on the first column if for some alarm is created notification.
### Actions with Factory Floors
#### View Configure all floors
Precondition: Factory floors are configured ([Configure Factory Floors](#_Configure_Factory_Floors)). Machines are added to factory floors and layout is saved. 

Click on **Configure icon** at the top right of organization tree opens tabs: Configure and Factory layout are shown. In the factory layout is possible to go to different floors.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.042.png)

*Figure 40: Factory layout - go to next floor*
#### Zoom in and Zoom out
Precondition: Factory floors are shown at the factory layout area. It is possible to zoon in or zoom out the floor area to see better the machines and their locations. When mouse is over some machine the zoom is executed and machine remains at the center of the layout.
#### Change point of view on floor
Precondition: Factory floors are shown at the factory layout area. 

Clicking on picture uploaded for factory floors is possible to move floors in the design map area to change point of view. 
#### Save the floor layout
Precondition: Factory floors are designed with added machines.

Click on the **Save** button to save floors layouts.
### Visualize Factory Layout
Precondition: Factory floors with machines are configured in Upkip Administration. 

Log in Upkip Visualization following the steps in [Upkip Visualization Sign in](#_Upkip_Visualization_Sign)

Selecting from main menu **Factory Layout** opens dashboard Factory Layout.

- Automatically are visible on factory layout configured floors with machines
- All functionalities of factory layout have to work with added machines
- If machine has status connected with animation it is executed