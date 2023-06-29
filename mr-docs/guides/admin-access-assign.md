---
title: Assign ownership of a guide in Dynamics 365 Guides
description: Learn how to assign ownership of a guide in Microsoft Dynamics 365 Guides.
author:  Mamaylya
ms.topic: conceptual
ms.date: 04/05/2022
ms.author: mamaylya
ms.reviewer: v-wendysmith
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
|Learn how privileges and access work| [How access to a record (guide) is determined](/power-platform/admin/how-record-access-determined)|
|Learn about the three types of teams (*owner* team, Azure Active Directory *group* team, or *access* team)|[Manage teams](/power-platform/admin/manage-teams)|
|Control access to the Dynamics 365 Guides HoloLens app or PC app|[Security roles and privileges](/power-platform/admin/security-roles-privileges#team-members-privilege-inheritance)|
|Control access to the Guides model-driven app| [Share a model-driven app using Power Apps](/powerapps/maker/model-driven-apps/share-model-driven-app)|

## Assign a guide to a user or an owner team

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. Select the guide that you want to assign. You can select multiple guides.

   ![Select the guide that you want to reassign.](media/admin-access-assign-01.PNG "Select the guide that you want to reassign")

1. Select **Assign**.

   ![Select assign a guide.](media/admin-access-assign-02a.PNG "Select assign a guide")

1. In the **Assign Guide** dialog box, to the right of the **Assign to** column, do one of the following:

    - Select **User or team** and then enter the name of the user or team (or use the search box) you want to assign the guide to. To create a new user or team, select **New Record**.

      ![Use the lookup to reassign a guide.](media/admin-access-assign-04a.PNG "Use the lookup to reassign a guide")

      > [!NOTE]
      > You must have admin permissions to see the **New Record** button.

    - Select **Me** to assign the guide to yourself. Keep in mind that you must be a system administrator to re-assign ownership of a guide that belongs to someone else.

1. Select **Assign** when you're done.

## Share a guide with someone else

Teams should be structured so that ownership of a guide is assigned to one or more teams that include the groups of users who need to collaborate on guides as authors, or use the guides as operators. In exceptional cases, you can use the **Share** option for individuals who are not members of a team. For details on the sharing process, see [Use access teams to limit access to specific guides or guide content in Dynamics 365 Guides](/dynamics365/mixed-reality/guides/admin-access-teams).

> [!NOTE]
> When you share a guide, the content (images, videos, and 3D objects) associated with the guide is not automatically shared. You can use the **All Content** tab in the Guides model-driven app to do bulk operations, such as sharing content.
>
> ![Screenshot of All Content tab in the Guides model-driven app.](media/mda-all-content-tab.PNG "Screenshot of All Content tab in the Guides model-driven app")

## See also

- [Create an access team](admin-access-teams.md)
- [Assign an Operator or Author role to an individual user](assign-role.md)
- [Assign roles in bulk by using Active Directory groups](admin-assign-role-groups.md)
- [Restrict access to an environment by using security groups](admin-security.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
