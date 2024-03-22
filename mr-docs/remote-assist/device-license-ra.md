---
author: davepinch
description: Learn how to set up a Dynamics 365 Remote Assist device license for multiple technicians on a single device.
ms.author: davepinch
ms.date: 03/21/2024
ms.topic: how-to
title: Set up a Remote Assist device license for multiple technicians on a shared device
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Set up a Remote Assist device license for multiple technicians on a shared device

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

A Dynamics 365 Remote Assist device license allows multiple technicians to use Dynamics 365 Remote Assist on a single device using a shared user account. A common scenario is a device that is shared between technicians in a facility, especially where each technician might not have an individual user account.

You need one device license for each device that will be shared between technicians. To acquire device licenses, contact your partner or reseller.

> [!NOTE]
> When you set up a shared account for multiple technicians, data is collected for the shared account only. Data about a particular technician can’t be analyzed.

## Prerequisites

- Understand managing Microsoft 365 or Microsoft Entra ID user accounts
- Understand assigning licenses
- Understand assigning roles if using the Remote Assist model-driven app

## Create a shared account for each device

For each device, assign a Remote Assist device license to a user account that will be shared between the technicians using that device. The following steps use the Microsoft 365 admin center to set up the shared account. If you prefer to use Microsoft Entra ID instead, see [Assign licenses to users by group membership in Microsoft Entra ID](/entra/identity/users/licensing-groups-assign).

1. [Open the Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home).

1. [Create a new account and assign a device license](deploy-remote-assist.md#add-users-and-assign-licenses) instead of a per-user license.

   - Since this account isn't tied to a specific user, set a display name that reflects the location name or device name.

   - Select **Let me create the password** checkbox and clear the **Require this user to change their password when they first sign in** checkbox and set up a shared password.

   - On the **Optional settings** page, leave the **User (no administrator access)** checkbox selected. A shared account shouldn't have administrator privileges.

1. [Deploy Remote Assist](deploy-remote-assist.md#deploy-dynamics-365-remote-assist).

## Assign a OneDrive license (optional)

If you want to use OneDrive on the shared device, assign a OneDrive license to the shared user account. All individuals using the shared account have access to the same OneDrive contents.

## Grant environment access (optional)

If you're using the Remote Assist model-driven app, then [add the shared user account](asset-capture-add-users.md) to the Dynamics 365 environment where the app is installed.

## Deploy the shared account

You can deliver the user account to your technicians as you normally would. However, we recommend that you prepare the device and streamline access to Remote Assist. You can also configure the device with a PIN, so you don’t have to share the account password.

1. Sign into the device with the shared account. If necessary, update the password.

1. Set a PIN so technicians can enter a PIN instead of a password.

1. Sign into Remote Assist and [test a call with another Teams user](making-taking-calls-hololens.md).

1. If you're using OneDrive, confirm the ability to [take a picture and save to OneDrive](take-snapshot-save-booking-hololens.md).

1. If you're using the model-driven app, [confirm calls are recorded](calls-dashboard.md). Calls are recorded from the shared user account, not from the individual using the shared account.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
