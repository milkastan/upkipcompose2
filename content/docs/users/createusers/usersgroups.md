---
title: "Users and Groups"
date: 2021-05-20T15:38:36+03:00
draft: false
weight: 3
---

### Create Users and Groups in Upkip
**Purpose**: Users and groups in the Upkip can be created by the user with role **System administrator** from the Upkip Administration.

Precondition: Log in the Upkip Administration as user system administrator

- User sees organizations and menu **Users and Groups.** 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.005.png)

*Figure 3: Upkip Administration - Home page*

Click on the button **USERS AND GROUPS**

- Form for creating users and groups is opened.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.006.png)

*Figure 4: Upkip Administration - Create users and groups*

#### Create or Delete Groups
**Purpose**: Created groups in AAD are related to some department(s) or whole factory. They are used for limiting user rights only to some department(s) or to the whole factory in the Upkip Visualization.

Selecting tab **Department groups** user is possible to create or delete groups.

Entering group name in **Create group** and click **Create**. 

- The new group is added in **Azure Active Directory /Groups.** The new group is visible in the drop down for deleting groups.

From the Select group in **Delete group** section select the newly created group and click **Delete**.

- The group is deleted from Azure Active Directory/Groups
#### Create User in Upkip
**Purpose**: User can create new users in the Upkip from Upkip Administration by automatically using azure functionality **Create user.**

Precondition: User with role system administrator is logged in Upkip Administration. Click on the menu **Users and Groups.** Click on the tab **Create User**. 

- Form for creating users in Upkip is opened

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.007.png)

*Figure 5: Upkip Administration - Create new user*

Reading the help information create properly user name. Enter the user data:

- **User name**
- **Password**
- **Names**
- **Role** – select from roles list
- **Group** – select from groups list

After filling all fields, Create button is enabled. Click **Create**. 

- The user should be created successfully if all information is added
- User is created in azure active directory
- User is added to select group
- User is synchronized with Upkip Administration and Upkip Visualization and can log into the applications
#### **Invite User in Upkip**
**Purpose**: User can create new users in the Upkip from Upkip Administration by automatically using azure functionality Invite user.

Precondition: User with role system administrator is logged in Upkip Administration. Click on the menu **Users and Groups.** Click on the tab **Invite User**. 

- Form for inviting users in the Upkip is opened

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.008.png)

*Figure 6: Upkip Administration - invite users*

.Enter the user data:

- **Name –** user names
- **Password**
- **Email** – user email
- **Role** – select from roles list
- **Group** – select from groups list

After filling all fields, **Invite** button is enabled. Click **Invite**. 

- The user will be emailed an invitation they can accept 
- User received also information email from Upkip with instructions how to accept invitation.

User has to click **Accept Invitation** in received email. If user has not Microsoft account, he is guided to create Microsoft account.

User **logs with its Microsoft account** and click **Accept** button. 

- The new user is created in AAD and appears in **AAD All users list** 

- User is added to select group
- User is synchronized with Upkip Administration and Upkip Visualization and can log into the applications


### Upkip Visualization Sign in
As a result of synchronization started in Upkip Administration

- The new user automatically is added to the corresponding team in the Upkip Visualization (The team is related with assigned role in AAD)

**Sign in with Azure AD** in the Upkip Visualization as a new created user

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.009.png)

*Figure 7: Upkip Visualization login form*

Click on the button **Sign in with Azure AD** button, enter username and password of the Microsoft account.

- The new user is logged in the Upkip Visualization
- The user see dashboards depending on their role 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.010.png)

*Figure 8: Upkip Visualization Home page*

To check if created user is added to the team in Upkip Visualization, log as a user with role system administrator. Select menu **Teams**.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.011.png)

*Figure 9: Upkip Visualization - Open Teams page*

- Teams page is opened

Click on some **Team** – e.g. Manager (if new user has role Manager)

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.012.png)

*Figure 10: Upkip Visualization - Open Team page*

- Team page is opened – e.g. Teams/Manager page
- User is added to the team (e.g. with role Manager)

### Upkip Administration Sign in
Precondition: To log in the Upkip Administration user should have assigned role System Administrator or Organization Administrator.

Navigate to Upkip Administration login page.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.003.png)

*Figure 11: Upkip Administration Login page*

Click on the button **Sign in with Microsoft**. Enter Microsoft account user name and password.

- Upkip Administration Home page is opened. 

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.013.png)

*Figure 12: Upkip Administration Home page*

To sign out from Upkip Administration click on the top right button. 

- User is logged out of Upkip Administration

The main elements of the page are:

- Vertical menus (collapsible)
- Organization tree structure with factory, departments, machines
- Factory floors layout with machines (Factory Layout is visualized in Upkip Visualization

To sign out from Upkip Administration click on the top right button. 

- User is logged out of Upkip Administration