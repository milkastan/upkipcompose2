---
title: "View and edit users"
date: 2021-05-20T15:42:08+03:00
draft: false
weight: 4
---
### **Edit User role in Upkip**
**Purpose**: User role in the Upkip platform can be edited in Azure Active Directory (AAD) and then synchronized with Upkip. The role of the user is updated in Upkip Administration and in Upkip Visualization.

Precondition: User with role System Administrator is logged in AAD of the Azure Subscription where the system is installed. 

Navigate to the **Azure Active Directory** à **Enterprise applications**. Select **i4based-administration application**. Select menu **Users and groups**. 

Find the user by filtering the list, select by checkmark and click **Edit**.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.014.png)

*Figure 13: AAD Edit user role for Upkip Administration*

1) Click to select new role from the list. Select new role and click button **Select**. Then click **Assign**. 
   1. The new role is assigned to user
### **Synchronize Users in Upkip**
After editing  user role in ADD or deleting user from AAD subscription is necessary **to synchronize user with Upkip applications.**

The users list is visible in the **Upkip Administration**. 

Sign in **Upkip Administration** as a user with role system administrator with Microsoft account.

Select **Organization.** Click on **Users** button at right.

![](/images/Aspose.Words.c55b6b06-cf77-4ce6-bf35-b1bd3972243e.015.png)

*Figure 14: Upkip Administration - Open users form*

- Users list of the Upkip organization is opened.

To synchronize the user(s) click the button **Synchronize**. 

- User(s) is added in the Upkip Configuration database
- User(s) is visible in the users list with location **Synced**. 
- User can log in the **Upkip Administration** if has role System Administrator or Organization Administrator
- User automatically is added in **Upkip Visualization** team depending on its role (The teams are Operator, Team Leader, Supervisor, Manager, System Administrator, Organization Administrator)    
### **Delete User from Upkip**
**Purpose**: User can be deleted from Upkip platform by deleting in Azure Active Directory (AAD) and then by synchronization removed from Upkip databases.

User with role System Administrator is logged in AAD of the Azure Subscription where the system is installed. 

Navigate to the **Azure Active Directory** à **All Users**. Search for a userà check the user and click **Delete user**à Confirm “Delete selected user?” with OK.

- User is successfully deleted from AAD

Log as System Administrator in Upkip Administration. Open users list and click button **Synchronize**.

- Deleted user in AAD is also removed from Upkip Configuration database.
- User is removed from Upkip Administraion
- User is removed from Upkip Visualization.
