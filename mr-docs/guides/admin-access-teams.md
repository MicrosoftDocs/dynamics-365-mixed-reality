---
author: melissahellmund
description: Learn how to create an access team to share a guide in Microsoft Dynamics 365 Guides.
ms.author: mehellmu
ms.date: 11/08/2023
ms.topic: how-to
title: Create an access team to share a guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Create an access team to share a guide in Dynamics 365 Guides

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

[Assigning ownership of a guide](admin-access-assign.md) to a user or team in Microsoft Dynamics 365 Guides is the preferred method for controlling who can use specific guides. If teams change frequently, however, resulting in a need to create and delete teams often, a Dynamics 365 admin (or other user with the Share privilege) can create a special type of team called an *access team* and share a guide through that team to control who can see specific guides and guide content (3D models, images, or videos).

For more information on the three types of teams (owner team, Microsoft Entra group team, or access team), see [Manage teams](/power-platform/admin/manage-teams).

> [!IMPORTANT]
> If you have already restricted access to guides or guides content by creating your own security role with reduced privileges, you’ll need to remove that security role and replace it with one of the [built-in security roles](admin-role-types.md).

## Create an access team

> [!TIP]
> You can associate a user with more than one access team.

1. In the [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), [create an access team](/power-platform/admin/manage-teams) in the Guides environment.

1. Select [**Add members to the team**](/power-platform/admin/manage-teams#manage-team-members).

1. After creating the access team, you can [share a guide with the access team](admin-share-guide.md).

## See also

- [How access to a record (guide) is determined](/power-platform/admin/how-record-access-determined)
- [Restrict access to an environment by using security groups](admin-security.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
