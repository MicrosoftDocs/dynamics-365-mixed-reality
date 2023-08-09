---
author: davepinch
description: Learn how to set up a Dynamics 365 Guides device license for multiple operators on a single HoloLens device.
ms.author: davepinch
ms.date: 02/01/2023
ms.topic: how-to
title: Set up a Dynamics 365 Guides device license
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Set up a Dynamics 365 Guides device license for multiple operators on a shared HoloLens device

A device license in Dynamics 365 Guides allows multiple operators to use Dynamics 365 Guides on a single device under a shared user account. This type of license is useful in scenarios where operators may not be known ahead of time (such as a classroom). It can also save licensing costs for customers with many operators that require infrequent access to the device. Device licenses can be purchased through your Microsoft account manager or reseller.

> [!NOTE]
> When you set up a shared HoloLens device for multiple operators, data collected is for the device only (HoloLens 1 device, for example). No user-specific data is captured. [Learn more about what data is collected in Dynamics 365 Guides](analytics-data-collected.md).

## Prerequisites

- The Guides solution has been [deployed and the apps set up](setup.md).

- You are familiar with the process of assigning licenses, assigning roles, and creating guides for use by operators.

- A working environment is available to test your device license.

## Create a shared account

A Dynamics 365 Guides device license must be assigned to a shared Active Directory user account. A shared account is just like a regular user account except it's shared by all people using Dynamics 365 Guides on a specific HoloLens device. Since the account is shared by multiple people, you manage credentials and other account details differently than regular accounts.

1. [Open the Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

1. [Add a user](/microsoft-365/admin/add-users).

   - On the **Set up the basics** page, fill in the first name, last name, display name, and username of the shared user account. Since this account is not tied to a specific user, you may want to identify the user by location name, device name, and so on.

   - On the **Set up the basics** page, select the **Let me create the password** check box and clear the **Require this user to change their password when they first sign in** check box. Set a shared password since this is a shared account. Otherwise, the first operator using the account will be prompted to select a password.

   - On the **Assign product licenses** page, select the location for the shared account, and then, under **Licenses**, select the **Dynamics 365 Guides** check box. 

   - On the **Optional settings** page, leave the **User (no administrator access)** check box selected. A shared operator account should not have administrator privileges.

   - Scroll down, expand the **Profile info** section, and fill in any profile information that will help you manage the shared account.

   - Review the information on the last page. To make changes, select the **Edit** button below the relevant sections. When you're finished, select **Finish adding**.

   - Make a note of the password. You (and the guide operators) will need this password to sign in.

## Assign an operator role to the shared account

[Assign either the **Dynamics 365 Guides Operator** or **Dynamics 365 Guides Restricted Operator** role to the shared account](assign-role.md#assign-roles-to-a-user). Assigning a role gives the account permission to use the HoloLens app to view and operate a guide. For more information on the different roles, see [About the Author and Operator roles.](admin-role-types.md)

## Grant access to a restricted environment (optional)

If you restricted your Microsoft Dataverse environment as described in [Restrict access to an environment in Dynamics 365 Guides by using security groups](admin-security.md), add the shared account to the security group. For more information, see [Control user access to environments: security groups and licenses](/power-platform/admin/control-user-access).

## Test the device license

Test the device license by operating a guide on the HoloLens with the shared account. This will also validate your password and optionally cache the credentials for use by your operators.

1. If you need to create a test guide, [sign into the PC app with an author or admin account](install-sign-in-pc-app.md#sign-in-to-the-app) so you can create a guide. For quick testing, [anchor the guide using a holographic anchor](pc-app-anchor-holographic.md) since this type of anchor doesn’t require a QR code printout.

1. Make sure your shared account has access to the test guide. This should happen automatically if you assigned the **Dynamics 365 Guides Restricted Operator** or **Dynamics 365 Guides Operator** role to the shared account. Otherwise [assign](admin-access-assign.md) or [share](admin-access-teams.md) the guide.

1. Put on your HoloLens and [sign in to the Dynamics 365 Guides HoloLens app](hololens-app-install-sign-in.md) using the shared operator account.

1. Since this will be the first time using the shared account, you may get prompted to reset the password (depending on how you set up the account).

   > [!TIP]
   > If you're prompted to select **Author** or **Operator**, you probably assigned an incorrect role to the account, or you're not signed into the app with the right account.

1. Respond to any prompts, and then [find and open the guide](find-guide.md).

1. When the guide opens, you'll be prompted to set the holographic anchor. If you reach this stage, your shared operator account is set up correctly.

## Next steps

- [Guides device license FAQ](device-license-faq.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
