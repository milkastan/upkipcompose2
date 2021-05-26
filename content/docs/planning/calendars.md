---
title: "Calendars"
date: 2021-05-20T15:50:28+03:00
draft: false
weight: 21
---

**Purpose:** In the calendars functionality is possible to create shift  templates that can apply to machines in the factory. Shift template defines working hours for machine and planned brakes. There is possible to create many shift templates. When assigning shift template to machine is necessary to select Active from – when this shift template is active for machine. 

Precondition: User with role Administrator is logged in the Upkip Administration.

Select menu **Calendars.**

- Calendars page is opened. By default is opened **Machine Calendar** tab. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.083.png)

*Figure 81: Upkip Administration - Calendars*

### Create Template
**Purpose:** In the page is possible to create new empty shift template by entering template name or create new shift template by copy hours from existing. 

Precondition: Calendars page is opened in the Upkip Administration.

Select tab **Create Template.**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.084.png)

*Figure 82: Upkip Administration - Calendars - Create template*

Enter in Template name the name of the new shift template. 

If nothing is selected from down with existing templates and click Create:

- New empty shift template is created. 

If select from drop down to copy from existing template and click Create:

- New shift template is created with hours copied from selected existing shift template.

### Shift Templates
**Purpose:** By this functionality is possible to define hours for created shift templates in the factory.

Precondition: There is created new empty shift template 

Select tab **Shift Templates**.

- On the left side is shown the list of created shift templates.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.085.png)

*Figure 83: Upkip Administration - Calendars - Shift templates*

If selecting some template from the list, at the right side is possible to define working hours and breaks. There is possible to define up to four shifts.

When entering hours for one day (for example Monday) and selecting **TUE** to define hours for Tuesday. If select at the bottom **Copy from day: Monday** and click **Copy**.

- The planned hours for Monday are copied to Tuesday.  By this way can copy hours for all working days in the week. 

There is possible to select **Timezone** from the list.

- **Shift Template is ready** with defined hours and timezone. 

Repeating the steps is possible to define many shift templates for the factory. 

### Machine Calendar
**Purpose:** By this functionality at the left are listed all configured machines in the factory. By selecting machine from the list is possible to assign created shift template and select active from date. For each machine in the factory is possible to apply shift calendar. 

Select tab **Machine Calendar.**

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.086.png)

*Figure 84: Upkip Administration - Calendars - Assign calendar to machine*

To apply calendar for machine follow the steps:

1) Select machine from the list
1) Select shift template from drop down list
1) Select **Active from** : date and time when shift template becomes active.
   - Shift template is assigned to machine.

Repeat the steps for all machines from the list.

### Downtime
**Purpose:** The defined shift template assigned to machine defines the machine working hours. During this time machine could have working status or untagged. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.087.png)

*Figure 85: Upkip Administration - Downtime of machine with assigned calendars*

**Downtime period types** are colored with different colors and could be: **unplanned, untagged and OK.** 

For periods **not included in the shift calendar** machine have status **Unplanned.**

- **Unplanned (grey)**  - The time when the machine was not planned to produce, according to the shift calendar. Unplanned time is **any time out of the shift or during breaks**.

For period **planned in the shift calendar** machine could have statuses – **OK or Untagged.**

- **Untagged (yellow)** - A period that is subject to tagging with a downtime reason by the system operator who is the responsible to provide explanation up the chain on the reason why the machine has not been producing in a period when it has been planned to. Low level of production time would mean high level of downtime, which could be explained by analyzing the top downtime reasons. The downtime tagging reasons are grouped in 4 groups: Man, Machine, Method and Material. 
- **OK** (green) - A period that is not considered as downtime and typically originates from the following machine statuses: Active, Machine offline, Machine online, System offline, System online. 

