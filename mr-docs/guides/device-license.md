---
author: prashantyvr
description: Learn how to set up a Dynamics 365 Guides device license for multiple operators on a single HoloLens device.
ms.author: prashan
ms.date: 04/25/2024
ms.topic: how-to
title: Set up a Guides device license for multiple operators
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Set up a Guides device license for multiple operators

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

A Dynamics 365 Guides device license allows multiple operators to use Dynamics 365 Guides on a single device under a shared user account. A device license is limited to operating a guide (no authoring can occur). Purchase device licenses through your Microsoft account manager or reseller.

> [!NOTE]
> When you set up a shared HoloLens device for multiple operators, data collected is for the device only. No user-specific data is captured. [Learn more about what data is collected in Dynamics 365 Guides](analytics-data-collected.md).

## Prerequisites

- [Deploy your Guides solution and apps](setup.md).
- Understand assigning licenses, assigning roles, and creating guides for use by operators.

## Create a shared account

A Dynamics 365 Guides device license must be assigned to a shared user account. Since multiple people share the account, you manage credentials and other account details differently than regular accounts. The following steps use the Microsoft 365 admin center to set up the shared account. If you prefer to use Microsoft Entra ID instead, go to [Assign licenses to users by group membership in Microsoft Entra ID](/entra/identity/users/licensing-groups-assign).

1. [Sign in to the Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

1. [Add users and assign licenses at the same time](/microsoft-365/admin/add-users/add-users).

   - Since this account isn't tied to a specific user, set a display name that reflects the location name or device name.

   - Select **Let me create the password** check box and clear the **Require this user to change their password when they first sign in** check box and set up a shared password.

   - On the **Optional settings** page, leave the **User (no administrator access)** check box selected. A shared account shouldn't have administrator privileges.

## Assign an operator role to the shared account

Assigning a role gives the account permission to use the HoloLens app to view and operate a guide.

1. [Assign an operator role](assign-role.md#assign-roles-to-a-user) to the shared account.

1. Choose either the **Operator** or **Restricted Operator** role. [Learn about the Author and Operator user roles](admin-role-types.md).

   The **Restricted Operator** role can access only guides that are explicitly shared or assigned to the account by an author. The **Operator** role has access to all guides and content in the environment.

## Grant access to a restricted environment (optional)

If you [restricted your Microsoft Dataverse environment by using security groups](admin-security.md), add the shared account to the security group.

## Test the device license

Test the device license by operating a guide on the HoloLens with the shared account. The test also validates your password and optionally caches the credentials for use by your operators.

1. If you need to create a test guide, [sign into the PC app with an author or admin account](install-sign-in-pc-app.md#sign-in-to-the-app) so you can create a guide. For quick testing, [anchor the guide using a holographic anchor](pc-app-anchor-holographic.md) since this type of anchor doesn’t require a QR code printout.

1. Make sure your shared account has access to the test guide. If you assigned the **Operator** role to the shared account, access happens automatically. Otherwise [assign](admin-access-assign.md) or [share](admin-access-teams.md) the guide.

1. Put on your HoloLens and [sign in to the Dynamics 365 Guides HoloLens app](hololens-app-install-sign-in.md) using the shared operator account.

1. Since it's the first time using the shared account, you might be prompted to reset the password (depending on how you set up the account). Respond to any prompts, and then [find and open the guide](find-guide.md).

1. When the guide opens, you're prompted to set the holographic anchor. Your shared operator account is set up.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
