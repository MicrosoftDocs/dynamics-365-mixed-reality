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

To add users to Dynamics 365 Guides, first assign a Guides license to each new or existing user. You can use the Microsoft 365 admin center, Microsoft Entra ID, or Microsoft Entra security groups.

We recommend using [Microsoft Entra security groups](/entra/fundamentals/concept-group-based-licensing) to assign licenses, add users, and assign Guides security roles at the group level. This option makes it easier to organize and manage user roles. To add users and assign licenses with an Entra security group, see [Use Microsoft Entra groups to add users, assign licenses, and assign roles.](admin-assign-role-groups.md)

This article explains how to add users and assign licenses with Microsoft 365 admin center or Microsoft Entra ID.

## Prerequisites

- You must have an [active Dynamics 365 Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](install-guides.md).

## Assign licenses and add individual users

Choose how you want to assign licenses and users.

- [Add users and assign licenses with Microsoft 365 admin center](/microsoft-365/admin/add-users/add-users)

- [Add users and assign licenses with Microsoft Entra ID](/azure/active-directory/fundamentals/license-users-groups)

> [!IMPORTANT]
> Regardless of how you assign licenses, make sure each user or group is assigned Dynamics 365 Guides, Common Data Service, and PowerApps for Guides.

## Next step

- [Assign the Guides security roles to each user](assign-role.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]