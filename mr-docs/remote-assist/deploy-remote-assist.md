---
title: Deploy Dynamics 365 Remote Assist
author: davepinch
description: Dynamics 365 Remote Assist users can deploy and set up Dynamics 365 Remote Assist on their devices. 
ms.author: davepinch
ms.service: dynamics-365-remote-assist
ms.date: 02/16/2023
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Deploy Dynamics 365 Remote Assist

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

After you get your [free trial](try-remote-assist.md) or [purchase](buy-remote-assist.md) Dynamics 365 Remote Assist or Dynamics 365 Remote Assist Attach (for Field Service customers), deploy it to your organization. To deploy:

- IT Admins assign licenses to users in your organization
- Individual users in your organization download and install the app on a [supported device](./requirements.md)

You can also [deploy to multiple tenants](multi-tenant-deployment.md) or [enable vendors and contractors to use Dynamics 365 Remote Assist](vendor-use-RA.md).

## Add users and assign licenses

There are two types of users for Dynamics 365 Remote Assist and Dynamics 365 Remote Assist Attach:

- Field service technicians who require a Dynamics 365 Remote Assist license, which also includes the required Microsoft Teams license.
- Remote experts (who aren't in the field) require only a Microsoft Teams license.

### Prerequisites

Your organization must have:

- A Microsoft 365 or Microsoft 365 [administrator account](https://www.microsoft.com/microsoft-365/business/office-365-administration). [Learn more about admin permissions](/office365/admin/admin-overview/admin-overview).

- A [free trial](try-remote-assist.md) of Dynamics 365 Remote Assist, or a [purchased license](buy-remote-assist.md).

Individual users in your organization must have:

- The [required licensing and devices](./requirements.md).

- An Azure Active Directory account to sign in to the app.

### Add and assign licenses

Add and assign licenses to *individual users* or a *group of users* in your organization through the Microsoft 365 or Microsoft 365 administrator portal.

1. Sign in to the [Microsoft 365 or Microsoft 365 administrator portal](https://www.microsoft.com/microsoft-365/business/office-365-administration) using your organization’s admin account.

1. Add and assign licenses:
   - To add a user and assign a license at the same time, see [Add users and assign licenses at the same time](/office365/admin/add-users/add-users). In the **Product licenses** section, make sure to provide them with Dynamics 365 Remote Assist and Microsoft Teams licenses.

   - To add multiple users at the same time, see [Add multiple users at the same time](/microsoft-365/admin/add-users/add-users#add-multiple-users-at-the-same-time-in-dashboard-view).

   - To assign licenses to existing users, see [Assign licenses to users](/office365/admin/manage/assign-licenses-to-users).


## Download and install the app

After assigning licenses, users can install and use the app on their HoloLens, HoloLens 2, or mobile devices.

### Prerequisites

- [A Dynamics 365 Remote Assist license **and** Microsoft Teams license assigned](#add-users-and-assign-licenses).

- A [Microsoft Teams account](https://teams.microsoft.com/start). See [Using Teams with Dynamics 365 Remote Assist](/dynamics365/mixed-reality/remote-assist/set-up-teams) for more information.

- Azure Active Directory [Premium trial](https://azure.microsoft.com/trial/get-started-active-directory/) (for HoloLens users only).

- A HoloLens, HoloLens 2, or mobile device. See [Licensing and product requirements](./requirements.md).

### Steps for HoloLens and HoloLens 2

1. Go to the **Start** menu select **Dynamics 365 Remote Assist** to update or launch the app. If you don't find the app installed by default, go to the Microsoft Store and get it there.

1. Sign in to Dynamics 365 Remote Assist with your Microsoft Teams account. Your **Contacts** page displays. If you're using a free trial, a prompt to start your **Free Trial of Dynamics 365 Remote Assist** displays.

You can now use Dynamics 365 Remote Assist on your HoloLens or HoloLens 2. Next, [Learn how to make calls](making-taking-calls-hololens.md).

### Steps for mobile devices

1. Go to the appropriate iOS or Android app store.

1. Search for and download **Dynamics 365 Remote Assist** and launch the app.

1. Sign in to Dynamics 365 Remote Assist with your Microsoft Teams account. Your **Contacts** page displays. If you're using a free trial, a prompt to start your **Free Trial of Dynamics 365 Remote Assist** displays.

You can now use Dynamics 365 Remote Assist on your mobile device. Next, [Learn how to make calls](mobile-app/making-calls-with-ar.md).

> [!Note]
> For Enterprise environments that manage application deployments using an Mobile Device Management (MDM) provider, contact d365rafb@microsoft.com for assistance obtaining the Dynamics 365 Remote Assist mobile application binary.

## Next steps

- [Set up Microsoft Teams on a PC or mobile for various scenarios](set-up-teams.md)
- [Install the Dynamics 365 Remote Assist model-driven app](ra-webapp-install.md)
- [Learn about the platforms that Dynamics 365 Remote Assist is dependent on](faq-deploy.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
