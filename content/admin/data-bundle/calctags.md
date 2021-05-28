---
title: "Calculated tags"
weight: 19
layout: redirect
---

**Purpose**: Calculated tags are used to execute expressions on the base tag values and assign results to Result tag. To create the expression built in functions can be used.

### Base and Result Tags
Create **Base** and **Result** tags that will be used for definition of calculated tag. 

Select **Organization** and some machine under department – e.g. Legiomix

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.071.png)

*Figure 69: Upkip Administration -Edit machine -Select tags for base and result tag*

Add tag with type INT that will be used as **Base Tag** following the steps [Search and add Tag](/admin/data/#search-and-add-tag)

For example: 99.IntTest, Payload: testTeams

Add tag with type INT that will be used as **Result Tag**

For example: 99.CalcTest, Payload: calculatedtest

### Add Calculated Tag
**Precondition**: User is logged in Upkip Administration. Base and Result Tags are created. Select menu **Calculated Tags.**

- The page for configuring calculated tags is opened. There is possible to create, edit or delete calculated tags.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.072.png)

*Figure 70: Upkip Administration - Calculated Tags*

Click **New** button.

- Form for creating calculated tag is opened.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.073.png)

*Figure 71: Upkip Administration - Add new calculated tag*

Enter the following data in the form:

-  **Name** - Enter the calculated tag name
-  **Base** – select base tag by searching between tags (button Tag)   or search by Display Name or Payload.
-  **Result** – select result tag by searching between tags (button Tag)   or search by Display Name or Payload.
-  **Add expression** to execute over the base tag. There is possible to Add Function from the built in functions, use math, logical or operators for comparison, parentheses if necessary. In expression is possible to add additional tags.
-  **Expression Parameters** - There is possible to define expression parameters, that used in the expression.
-  Click **Add**
   - The calculated tag is created.

### Search for Base and Result Tags
-  When searching to add Base and Result tags there is possible to search tag from **all tags** or from **organization tree** following the steps [Search and Add Tag](/admin/data/events/#search-and-add-tag)

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.074.png)

*Figure 72: Upkip Administration - New Calculated tag - Select base and result tags*

-  When adding Base or Result Tags is possible to select not real tags but Display name with specific Type ID.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.075.png)

*Figure 73: Upkip Administration - New calculated tag - select tag by display name*

After adding tag or display name they are filled read only in the fields for Base tag and Result Tag

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.076.png)

*Figure 74: Upkip Administration - New calculated tag - Selected base and result tags*

### Add Expression
When creating calculated tag is possible to create expression that will be executed on the base tag. The result of execution will be written to Result Tag. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.077.png)

*Figure 75: Upkip Administration - New calculated tag - Add expression*

To create expression can be used:

-  [Built in Functions](/admin/data/calctags/#built-in-functions) – implemented functions that can be selected from the list.
-  [Add Tag](/admin/data/events/#search-and-add-tag) – it is possible to select tag from all tags or from organization tree to add in expression
-  [Add Display name](/admin/data/calctags/#search-for-base-and-result-tags) – it is possible to search and select display name of some Type and add in expression.
-  **Use mathematical or logical operations**, operators for comparison or parentheses to create expression.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.078.png)

*Figure 76: Upkip Administration - New calculated tag - Add expression operators*

-  There is possible to define expression parameters and use them in expression.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.079.png)

*Figure 77: Upkip Administration - New calculated tag - Add parameters*

Expression parameter has **Name, Type and Value.** Use in expression with its name. 

After filling the required fields – Name, Result, Base and Expression, click **Save**

- Calculated tag is saved and appears in the list of Calculated tags.

For example: 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.080.png)

*Figure 78: Upkip Administration - Saved calculated tag in the list*
#### Built in Functions
To add function in expression click on the button **+ Add Function.** 

- The list with predefined function is listed.  

When selecting some function at the right side appears Description and example.

Select some function and click **Add** button.

- The selected function appears in the expression section.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.081.png)

*Figure 79: Upkip Administration - New calculated tag - Add expression - Built in functions*


