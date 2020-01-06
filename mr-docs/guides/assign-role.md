---
author: Mamaylya
description: Assign Author or Operator roles to users in Dynamics 365 Guides to control whether users can edit and view guides (Author role) or just view guides (Operator role)
ms.author: mamaylya
ms.date: 01/28/2020
ms.service: crm-online
ms.topic: article
title: Assign an Author or Operator role to a user to control whether a user can author a guide or just view a guide (Operator role)
ms.reviewer: v-brycho
---

# Assign an Author or Operator role to a user

If you're an administrator, you can assign an **Author** or **Operator** role to a user to control whether they can view guides (Operator role) 
or view and edit guides (Author role).  

## Prerequisites
 
To modify user roles, you must have: 

- An active Dynamics 365 Guides license. For more information, see [Buy and deploy Dynamics 365 Guides](setup.md).

- The latest Dynamics 365 Guides solution installed. For more information, see [upgrade to the latest solution](upgrade.md). 

- Access to the Power Platform Admin center and full administrator privileges. 

## Assign user roles

1. Go to the [PowerPlatform Admin center](https://admin.powerplatform.microsoft.com/environments), and then sign in with your administrator credentials. 

2. Select **Environments** in the left pane (if the **Environments** page isn't already open).  

3. Select the environment you want to work with, select the **More environment actions** (...) button, and then select **Settings**.

   ![Environment settings](media/environment-settings.PNG "Environment settings")
 
4. Select **Users + permissions** to expand the list of options, and then select **Users**. If you're prompted to sign in to Dynamics.com, make sure to you use your administrator credentials. 
  
   A new window with your Dynamics 365 instance will appear. 
   
   ![Users dialog box](media/user-dialog.PNG "Users dialog box")
 
5. Select a user or multiple users, and then select **Manage Roles** at the top of the screen. 
  
   ![Manage Roles](media/manage-roles2.PNG "Manage Roles")

6. In the **Manage User Roles** screen, make sure that the **Common Data Service User** is selected. This option should 
be enabled by default.

   ![Common Data Service User check box](media/marker-spacing.png "Common Data Service User check box")
 
7. Select the appropriate check box (list options here), and then select **OK**. 

   ![Author and Operator check boxes](media/author-operator-check-boxes.PNG "Author and Operator check boxes")

### See also

[Author a guide](authoring-overview.md)<br>
[Operate a guide](operator-guide.md)

