---
author: davepinch
description: Add user accounts to a Microsoft Dynamics 365 Guides license.
ms.author: davepinch
ms.date: 12/04/2023
ms.topic: how-to
title: Assign licenses and add users
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Assign licenses and add users

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

When assigning licenses and adding users, you must:

- Assign licenses to individual users or a group of users
- Assign security roles to those users or group
- Link the users or group to the Guides environment through a Dataverse group

We recommend using [Microsoft Entra security groups](/entra/fundamentals/concept-group-based-licensing) to assign licenses, add users, and assign Guides security roles at the group level. This option makes it easier to organize and manage user roles. By linking Microsoft Entra security groups  to a Dynamics 365 group team, Dynamics 365 Guides roles can be inherited by any user added to the Microsoft Entra group.

If you choose not to use Entra security groups, you can assign licenses to individual users using [Microsoft 365 admin center](#add-users-and-assign-licenses-with-the-microsoft-365-admin-center) or [Microsoft Entra ID](#add-users-and-assign-licenses-with-microsoft-entra-id). 

> [!IMPORTANT]
> Regardless of how you assign licenses, make sure each user or group is assigned Dynamics 365 Guides, Common Data Service, and PowerApps for Guides.

## Prerequisites

- You must have an [active Dynamics 365 Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](install-guides.md).

## Add users and assign licenses with a Microsoft Entra security group

You can create a Microsoft Entra security group add users to that group. Assign licenses to the group and then link the Entra security group to a Dataverse team group.

1. [Create a Microsoft Entra security group and add users.](/entra/fundamentals/how-to-manage-groups)

1. [Assign Guides licenses to the Entra security group.](/entra/identity/users/licensing-groups-assign)

1. [Create a Dynamics 365 group team](/power-platform/admin/manage-group-teams#create-a-group-team) in the environment where you installed the Guides solution, linking the group to the Microsoft Entra security group you created.

## Add users and assign licenses with Microsoft 365 admin center

[Add users and assign licenses with Microsoft 365 admin center](/microsoft-365/admin/manage/assign-licenses-to-users)

## Add users and assign licenses with Microsoft Entra ID

[Add users and assign licenses with Microsoft Entra ID](/azure/active-directory/fundamentals/license-users-groups)

## Next steps

- [Assign the Guides security roles](assign-role.md) for each user.
- [Assign the Dynamics 365 Guides security roles](/power-platform/admin/manage-group-teams#manage-the-security-roles-of-a-team). For more information, see the [Author and Operator roles in Guides](admin-role-types.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]