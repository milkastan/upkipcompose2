---
title: "Users Management"
date: 2021-05-20T15:51:36+03:00
draft: false
weight: 2
---

The prime source of users is **Azure Active Directory (AAD)** of the Azure Subscription where the system is installed. The system resources are created within a dedicated Resource Group in that Azure Subscription. In the AAD a dedicated user group (Root User Group) is created where all users with access to the system should be added. The name of this user group is with the name of the Resource Group. 

**Important note:** All users (and groups) members of the Root User Group are automatically synced (periodically) with the system’s internal database.

{{< button "/docs/users/createusers/usersgroups/" "To Users and Groups" "mb-1" >}}

