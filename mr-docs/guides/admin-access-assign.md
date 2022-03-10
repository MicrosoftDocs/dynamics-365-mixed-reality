---
title: Assign ownership of a guide in Dynamics 365 Guides
description: Learn how to assign ownership of a guide in Microsoft Dynamics 365 Guides.
author:  MattHoag-MS
manager: tfehr
ms.topic: conceptual
ms.date: 04/05/2022
ms.author: v-mhoag
ms.reviewer: v-bholmes
---

# Assign ownership of a guide in Dynamics 365 Guides

When you create a guide in Microsoft Dynamics 365 Guides, you are automatically assigned as the owner of the guide. If you want to share ownership of the guide with others in your organization, you can:

- Assign ownership of the guide to another person. 

- Assign ownership of the guide to an owner team. 

- Keep ownership of the guide, but let someone else work on it with you by using the **Share** option.

> [!NOTE]
> You can also assign the ownership of a guide to yourself if you have a role with the Assign privilege. You must be a system administrator to re-assign ownership of a guide that belongs to someone else.

For more information on privileges, teams, and controlling access to apps, see the following articles.

|To|See this article|
|---------------------------------------|-----------------------------------------------------|
|Learn how privileges and access work| [How access to a record (guide) is determined](https://docs.microsoft.com/power-platform/admin/how-record-access-determined)|
|Learn about the three types of teams (*owner* team, Azure Active Directory *group* team, or *access* team)|[Manage teams](https://docs.microsoft.com/power-platform/admin/manage-teams)|
|Control access to the Dynamics 365 Guides HoloLens app or PC app|[Security roles and privileges](https://docs.microsoft.com/power-platform/admin/security-roles-privileges#team-members-privilege-inheritance)|
|Control access to the Guides model-driven app| [Share a model-driven app using Power Apps](https://docs.microsoft.com/powerapps/maker/model-driven-apps/share-model-driven-app)|

## Assign a guide to a user or an owner team

1. Go to [Dynamics 365 Home](https://home.dynamics.com/), and then select the **App launcher** button ![app launcher icon.](media/app-launcher-icon.png) in the upper-left corner of the window.

2. Select **Power Apps**, select **Apps**, and then select **Guides**.  

3. Select the guide that you want to assign. You can select multiple guides.
   
   ![Select the guide that you want to reassign.](media/admin-access-assign-01.PNG "Select the guide that you want to reassign")

4. Select **Assign**.

   ![Select assign a guide.](media/admin-access-assign-02a.PNG "Select assign a guide")

5. In the **Assign Guide** dialog box, to the right of the **Assign to** column, do one of the following:

    - Select **User or team** and then enter the name of the user or team (or use the search box) you want to assign the guide to. To create a new user or team, select **New Record**.
      
      ![Use the lookup to reassign a guide.](media/admin-access-assign-04a.PNG "Use the lookup to reassign a guide")

      > [!NOTE]
      > You must have admin permissions to see the **New Record** button. 

    - Select **Me** to assign the guide to yourself. Keep in mind that you must be a system administrator to re-assign ownership of a guide that belongs to someone else.    
      
      ![Select Me to assign the guide to yourself.](media/admin-access-assign03a.PNG "Select Me to assign the guide to yourself")    
      
6. Select **Assign** when you're done.

## See also

[Share a guide through an access team](admin-access-teams.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
