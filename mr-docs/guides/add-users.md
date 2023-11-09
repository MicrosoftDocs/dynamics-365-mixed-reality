---
author: davepinch
description: Add user accounts to a Microsoft Dynamics 365 Guides license.
ms.author: davepinch
ms.date: 10/12/2023
ms.topic: how-to
title: Assign licenses and add users
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Assign licenses and add users

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

As a Microsoft Dynamics 365 Guides admin, assign licenses to individual users or a group of users in your organization. Choose how you want to assign licenses to users and perform the appropriate task.

- Add users through Microsoft Entra ID. We recommend this option because you can assign licenses and Guides security roles at the group level.
- Add users manually through the Power Platform admin center and set security roles as you add the user.

> [!IMPORTANT]
> Make sure each user or group is assigned Dynamics 365 Guides, Common Data Service, and PowerApps for Guides.

## Prerequisites

- You must have an [active Dynamics 365 Guides license](buy-guides.md).

- The [Dynamics 365 Guides solution must be installed](install-guides.md).

### Add users and assign licenses with Microsoft Entra ID

1. [Create a Microsoft Entra security group.](/entra/fundamentals/groups-view-azure-portal)

1. [Assign Guides licenses to the group.](/entra/identity/users/licensing-groups-assign)

1. [Add users to the security group.](/entra/fundamentals/concept-group-based-licensing)



| Platform | How to |
|---|---|
|[Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/)| - [Assign licenses to existing users](/microsoft-365/admin/manage/assign-licenses-to-users)<br>- [Add users and assign licenses at the same time](/microsoft-365/admin/add-users/add-users)<br>- [Add multiple users and licenses at the same time](/microsoft-365/admin/add-users/add-users#add-multiple-users-at-the-same-time-in-dashboard-view)|
|[Azure Active Directory](https://portal.azure.com/)|- [Assign licenses to individual users](/azure/active-directory/fundamentals/license-users-groups)<br>- [Assign licenses to users by group membership](/azure/active-directory/enterprise-users/licensing-groups-assign)|

## Next step

- [Assign user roles](assign-role.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]