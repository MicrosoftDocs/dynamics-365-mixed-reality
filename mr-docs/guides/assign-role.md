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

If you're an administrator, you can assign an **Author** or **Operator** role to a user. The following table describes the privileges granted by each role.

|Role|Description|
|-----------------------|----------------------------------------------------------------------|
|Author|Use the PC app and HoloLens app to create, edit, and operate guides.|
|Operator|Use a guide. If the **Operator** role is set, operators can also save a step when opening a guide by skipping the **Select Mode** dialog box.|

## Prerequisites
 
To modify user roles, you must have: 

- An active Dynamics 365 Guides license. For more information, see [Try or buy, and deploy Dynamics 365 Guides](setup.md).

- The latest Dynamics 365 Guides solution installed. For more information, see [upgrade to the latest solution](upgrade.md). 

- Access to the Power Platform Admin center and full administrator privileges. 

## Assign user roles

1. Go to the [PowerPlatform Admin center](https://admin.powerplatform.microsoft.com/environments), and then sign in with your administrator credentials. 

2. Select **Environments** in the left pane (if the **Environments** page isn't already open).  

3. Select the environment you want to work with, select the **More environment actions** (...) button, and then select **Settings**.

   ![Environment settings](media/environment-settings.PNG "Environment settings")
 
4. Select **Users + permissions** to expand the list of options, and then select **Users**. If you're prompted to sign in to Dynamics 365, make sure to use your administrator credentials.   
      
   ![Users selected](media/users-setting.PNG "Users selected")
 
5. Select a user or multiple users, and then select **Manage Roles** at the top of the screen. 
  
   ![Manage Roles](media/select-manage-roles.PNG "Manage Roles")

6. In the **Manage User Roles** dialog box, make sure that the **Common Data Service User** check box is selected. 

   ![Common Data Service User check box](media/common-data-service-user.PNG "Common Data Service User check box")
 
7. Select the check box for the appropriate role for this user, and then select **OK**. 

   ![Author and Operator check boxes](media/select-role.PNG "Author and Operator check boxes")

### See also

[Overview of authoring a guide](authoring-overview.md)<br>
[Overview of operating a guide](operator-overview.md)

