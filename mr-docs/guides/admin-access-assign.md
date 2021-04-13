---
title: Assign a guide using owner teams to limit access to specific guides or guide content in Dynamics 365 Guides
description: Learn how to assign a guide to an owner team to limit access to specific guides or guide content in Dynamics 365 Guides.
author:  MattHoag-MS
manager: anhaman
ms.service: crm-online
ms.topic: conceptual
ms.date: 04/14/2021
ms.author: v-mhoag
ms.reviewer: v-bholmes
---
<!-- This article is a copy of the article below with the term "record" updated to "guide".   A better solution will have to be found to "customize" core power apps support documents to address the specific D365 Guides user experience.  
https://docs.microsoft.com/powerapps/user/assign-or-share-records -->

# Limit access to a specific guide or guide content in Dynamics 365 Guides by using owner teams

When you create a guide in Microsoft Dynamics 365 Guides, you are assigned as the owner of the guide. If you want another person in your organization to also have ownership of the guide, you can assign the ownership of a guide to that person. You can assign the ownership of a guide to a user or a team. You can also assign the ownership of a guide to yourself if you have a role with the Assign privilege.

If you want to keep ownership of the guide, but let someone else work on it with you, you can use the **Share** option to share the guide.

For more information, see the following articles.

|To|See this article|
|----------------------------------------------------|-----------------------------------------------------|
|Learn about how privileges and access work| [How access to a row (or guide) is determined](https://docs.microsoft.com/power-platform/admin/how-record-access-determined)|
|Learn about the three types of teams (*owner* team, Azure Active Directory *group* team, or *access* team)|[Manage Teams in Power Platform Security](https://docs.microsoft.com/power-platform/admin/manage-teams)|
|Provide access to the HoloLens app or PC app|[Security roles and privileges](https://docs.microsoft.com/power-platform/admin/security-roles-privileges#team-members-privilege-inheritance)|
|Control access to the Guides model-driven app| [Share a model-driven app using Power Apps](https://docs.microsoft.com/powerapps/maker/model-driven-apps/share-model-driven-app)|

## Assign a guide to a user or an owner team

1. Go to [Dynamics 365](https://home.dynamics.com/)  and open the App Launcher using the App Launcher icon  ![app launcher icon](media/app-launcher-icon.png) at the top left of the top menu bar.
1. Select **Power Apps** , then select **Apps**, and select **Guides**.  
1. From a list of guide, select the guide that you want to assign to someone else. You can select multiple guides.

   > [!div class="mx-imgBorder"]
   > ![Select the guide that you want to reassign](media/admin-access-assign-01.png "Select the guide that you want to reassign")

1. On the command bar, select **Assign**.

   > [!div class="mx-imgBorder"]
   > ![Select assign a guide](media/admin-access-assign-02.png "Select assign a guide")

1. In the assign dialog box, select the **Assign to** column, and choose one of the following options:
    - Select **Me** to assign the guide to yourself and then select **Assign**. Remember only a system administrator can re-assign ownership of a guide that belongs to someone else.
      > [!div class="mx-imgBorder"]
      > ![Select Me to assign the guide to yourself](media/admin-access-assign-03.png "Select Me to assign the guide to yourself")
    - Select **User or Team** and then enter the name of the user or team or use the lookup to find them. Or, select **New record** to create a new user or team. When you're done select **Assign**.

      > [!div class="mx-imgBorder"]
      > ![Use the lookup to reassign a guide](media/admin-access-assign-04.png "Use the lookup to reassign a guide")

## Share a guide with someone else

 Teams should be structured so that ownership of a guide is assigned to one or more teams that include the groups of users who need to collaborate on Guides as Authors, or use Guides as Operators. In exceptional cases, the share option can be used for individuals who are not members of a team.  For details on the sharing process see [Use access teams to limit access to specific guides or guide content in Dynamics 365 Guides](https://docs.microsoft.com/dynamics365/mixed-reality/guides/admin-access-teams).

[!INCLUDE[footer-include](../includes/footer-banner.md)]
