---
author: davepinch
description: Add user accounts to a Microsoft Dynamics 365 Guides license.
ms.author: davepinch
ms.date: 12/13/2023
ms.topic: how-to
title: Add licenses and users to individual users
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Add licenses and users to individual users

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

To add users to Dynamics 365 Guides, first assign a Guides license to each new or existing user. Then, in the Power Platform admin center, configure the roles that the users will have access to (Author, Operator, or Admin).

To assign licenses and add users, you can use the Microsoft 365 admin center, Microsoft Entra ID, or Microsoft Entra security groups.

We recommend using [Microsoft Entra security groups](/entra/fundamentals/concept-group-based-licensing) to add users, assign licenses, and assign roles. This option makes it easier to organize and manage user roles. Guides roles can be inherited by any user added to the Entra security group. To use this option, see [add licenses, users, and roles to Microsoft Entra security groups](admin-assign-role-groups.md).

## Prerequisites

- You must have an [active Dynamics 365 Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](install-guides.md).

## Assign licenses and add individual users

Choose how you want to assign licenses and users.

- [Add users and assign licenses with Microsoft 365 admin center](/microsoft-365/admin/add-users/add-users)

- [Add users and assign licenses with Microsoft Entra ID](/azure/active-directory/fundamentals/license-users-groups)

> [!IMPORTANT]
> Regardless of how you assign licenses, make sure each user or group is assigned Dynamics 365 Guides, Common Data Service, and PowerApps for Guides.

## Next steps

- [Assign the Guides security roles to each user](assign-role.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]