---
author: davepinch
description: Add user accounts to a Microsoft Dynamics 365 Guides license.
ms.author: davepinch
ms.date: 11/10/2023
ms.topic: how-to
title: Assign licenses and add users
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Assign licenses and add users

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

<!--- Work with Dave and Alwin to update 
As a Microsoft Dynamics 365 Guides admin, assign licenses to individual users or a group of users in your organization. Choose how you want to assign licenses to users: 

- Add users through Microsoft Entra ID. We recommend using Microsoft Entra ID. With this option, you can assign licenses and Guides security roles at the group level. Assigning licenses at a group level is optional. You can assign licenses to individual users.
- Add users manually through the Power Platform admin center and set security roles as you add the user.

--->

To add users to Dynamics 365 Guides, assign a Guides license to a new or existing user. You can use the Microsoft 365 admin center or Microsoft Entra ID to assign licenses. Then, in the Power Platform admin center, configure the Guides security roles for each user or security group.

> [!IMPORTANT]
> Make sure each user or group is assigned Dynamics 365 Guides, Common Data Service, and PowerApps for Guides.

## Prerequisites

- You must have an [active Dynamics 365 Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](install-guides.md).

### Assign licenses with Microsoft 365 admin center

1. Sign in to the [Microsoft 365 admin center.](https://admin.microsoft.com/AdminPortal/)

1. Assign licenses to users using one of the following processes:

   - [Assign licenses to existing users](/microsoft-365/admin/manage/assign-licenses-to-users)

   - [Add users and assign licenses at the same time](/microsoft-365/admin/add-users/add-users)

   - [Add multiple users and licenses at the same time](/microsoft-365/admin/add-users/add-users#add-multiple-users-at-the-same-time-in-dashboard-view)|

### Assign licenses with Microsoft Entra

1. Sign in to the [Microsoft Entra admin center.](https://entra.microsoft.com/)

1. Assign licenses to users using one of the following processes:

   - [Assign licenses to individual users](/azure/active-directory/fundamentals/license-users-groups)

   - [Assign licenses to users by group membership](/azure/active-directory/enterprise-users/licensing-groups-assign)|

<!--- Work with Dave and Alwin to update 

### Add users and assign licenses to a Microsoft Entra security group

You can create a Microsoft Entra security group and assign licenses to the group and add users to that group. Then, link the Entra security group to a Dataverse team group.

1. [Create a Microsoft Entra security group.](/entra/fundamentals/groups-view-azure-portal)

1. [Assign Guides licenses to the group.](/entra/fundamentals/license-users-groups)

1. [Add users to the security group.](/entra/fundamentals/concept-group-based-licensing)

1. [Create a Power Platform group team](/power-platform/admin/manage-group-teams) and link to the Microsoft Entra security group you created.  Point to admin assign role groups

--->

## Next step

- [Assign the Guides security roles](assign-role.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]