---
title: Deploy Dynamics 365 Remote Assist
author: davepinch
description: Dynamics 365 Remote Assist users can deploy and set up Dynamics 365 Remote Assist on their devices. 
ms.author: davepinch
ms.service: dynamics-365-remote-assist
ms.date: 05/08/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Deploy Dynamics 365 Remote Assist

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

Deploy Dynamics 365 Remote Assist to your organization. You can [deploy to multiple tenants](multi-tenant-deployment.md) or [enable vendors and contractors to use Dynamics 365 Remote Assist](vendor-use-RA.md).

## Prerequisites

- A [purchased Dynamics 365 Field Service license](/dynamics365/field-service/buy-fs), or a [trial](try-remote-assist.md) or [purchased Dynamics 365 Remote Assist license](buy-remote-assist.md).
- Individuals have a [supported device](./requirements.md).

## Add users and assign licenses

If you purchased Dynamics 365 Field Service, you can skip this step and have your users [download and install the app on their device](#download-and-install-the-app).

If you purchased Dynamics 365 Remote Assist or have a trial version, determine the types of users:

- Field service technicians who require a Dynamics 365 Remote Assist license, which also includes the required Microsoft Teams license.
- Remote experts (who aren't in the field) require only a Microsoft Teams license.

### Prerequisites

- Your organization must have a Microsoft 365 [administrator account](https://www.microsoft.com/microsoft-365/business/office-365-administration). [Learn more about admin permissions](/office365/admin/admin-overview/admin-overview).

- Individual users in your organization must have a Microsoft Entra account to sign in to the app.

### Add users and assign licenses

Add and assign licenses to *individual users* or a *group of users* in your organization.

1. Sign in to the [Microsoft 365 admin center](https://admin.microsoft.com/) using your organization’s admin account.

1. Add and assign licenses:
   - To add a user and assign a license at the same time, see [Add users and assign licenses at the same time](/microsoft-365/admin/add-users/add-users). Make sure to provide them with Dynamics 365 Remote Assist and Microsoft Teams licenses.

   - To add multiple users at the same time, see [Add multiple users at the same time](/microsoft-365/admin/add-users/add-users#add-multiple-users-at-the-same-time-in-dashboard-view).

   - To assign licenses to existing users, see [Assign licenses to users](/microsoft-365/admin/manage/assign-licenses-to-users).

## Download and install the app

Users can install and use the Dynamics 365 Remote Assist app on their HoloLens 2 or mobile devices.

### Prerequisites

- A [Dynamics 365 Remote Assist license **and** Microsoft Teams license assigned](#add-users-and-assign-licenses).

- A [Microsoft Teams account](https://teams.microsoft.com/start). Go to [Using Teams with Dynamics 365 Remote Assist](/dynamics365/mixed-reality/remote-assist/set-up-teams) for more information.

- A [Microsoft Entra account](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id) (for HoloLens users only).

### Steps for HoloLens 2

1. Go to the **Start** menu select **Dynamics 365 Remote Assist** to update or launch the app. If you don't find the app installed by default, go to the Microsoft Store and get it there.

1. Sign in to Dynamics 365 Remote Assist with your Microsoft Teams account. Your **Contacts** page displays. If you're using a free trial, a prompt to start your **Free Trial of Dynamics 365 Remote Assist** displays.

You can now use Dynamics 365 Remote Assist on your HoloLens 2. Next, [Learn how to make calls](making-taking-calls-hololens.md).

### Steps for mobile devices

1. Go to the appropriate iOS or Android app store.

1. Search for and download **Dynamics 365 Remote Assist** and launch the app.

1. Sign in to Dynamics 365 Remote Assist with your Microsoft Teams account. Your **Contacts** page displays. If you're using a free trial, a prompt to start your **Free Trial of Dynamics 365 Remote Assist** displays.

You can now use Dynamics 365 Remote Assist on your mobile device. Next, [Learn how to make calls](mobile-app/making-calls-with-ar.md).

> [!Note]
> For Enterprise environments that manage application deployments using a Mobile Device Management (MDM) provider, contact d365rafb@microsoft.com for assistance obtaining the Dynamics 365 Remote Assist mobile application binary.

## Next steps

- [Set up Microsoft Teams on a PC or mobile for various scenarios](set-up-teams.md)
- [Install the Dynamics 365 Remote Assist model-driven app](ra-webapp-install.md)
- [Learn about the platforms that Dynamics 365 Remote Assist is dependent on](faq-deploy.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
