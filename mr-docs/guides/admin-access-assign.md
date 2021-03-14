---
title: "Assign a guide using owner teams to limit access to specific guides or guide content in Dynamics 365 Guides | MicrosoftDocs"
description: How to Assign a guide to an owner team with power apps admin
author:  v-mhoag
manager: anhaman
ms.service: Guides
ms.component: pa-user
ms.topic: conceptual
ms.date: 11/10/2020
ms.author: v-mhoag
ms.custom: ""
ms.reviewer: ""
ms.assetid: 
search.audienceType: 
  - enduser
search.app: 
  - Guides
  - PowerApps
  - D365CE
---
<!-- This article is a copy of the article below with the term "record" updated to "guide".   A better solution will have to be found to "customize" core power apps support documents to address the specific D365 Guides user experience.  
https://docs.microsoft.com/powerapps/user/assign-or-share-records -->

# Assign or share guides

When you create a guide, you are the owner of the guide. If you would like another person in your organization to take ownership of the guide, then you can assign the guide to that person. You can assign a Guide to a user or team. You can also assign a guide to yourself that another user owns but you need to have system administrator privilege to do this.

If you want to keep ownership of the guide but let someone else work on it with you, then use the **Share** option to share the guide.

For more information on how privileges and access works, see [How access to a row (or guide) is determined](https://docs.microsoft.com/power-platform/admin/how-record-access-determined).

For more information on how to control access to Guides Hub which is a model-driven app, see [Share a model driven app using power app](https://docs.microsoft.com/powerapps/maker/model-driven-apps/share-model-driven-app).

For information on background to give access to the hololens app or PC App, see [Security roles and privileges](https://docs.microsoft.com/power-platform/admin/security-roles-privileges#team-members-privilege-inheritance)

For more information on the three types of teams; *owner* team, Azure Active Directory (Azure AD) *group* team, or an *access* team , see [Manage Teams in Power Platform Security](https://docs.microsoft.com/power-platform/admin/manage-teams).

## Assign a guide to a user or an owner team

1. Launch [Power Apps](https://make.powerapps.com/)  or open the App Launcher using the “ : : : “ icon at the left of the top menu bar,   select **Power Apps** , then select **Apps**, and select **Guides**.  
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

 If you want to keep ownership of a guide but let someone else work on the guide with you then use the share option see [Use access teams to limit access to specific guides or guide content in Dynamics 365 Guides](https://docs.microsoft.com/dynamics365/mixed-reality/guides/admin-access-teams).

[!INCLUDE[footer-include](../includes/footer-banner.md)]
