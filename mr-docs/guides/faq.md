---
author: davepinch
description: Frequently asked questions about Dynamics 365 Guides
ms.author: davepinch
ms.date: 04/28/2023
ms.topic: article
title: FAQ about Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Frequently asked questions about Microsoft Dynamics 365 Guides

[See also Dynamics 365 Guides 8.0 FAQ](faq-version-8.md)

## How do I contact Support if I don't find an answer in this FAQ?

If you're not able to use Microsoft Dynamics 365 Guides, or if you have an issue that isn't answered in this FAQ or in the documentation, please contact Customer Support by using the following steps:

1. Go to [https://dynamics.microsoft.com/support/](https://dynamics.microsoft.com/support/).

2. Under **Customer Engagement help + support**, select **GET SUPPORT**.

3. Find a phone number or submit a support request through the admin center. 

## Which Microsoft platforms is Dynamics 365 Guides dependent on?
 
Dynamics 365 Guides is dependent on three Microsoft platforms:
 
- Microsoft Dataverse
- Microsoft Dynamics 365 Core Service
- Microsoft Teams
 
In rare cases, changes to these underlying platforms can cause issues in Dynamics 365 Guides. Likewise, a change to one of these platforms can resolve a Dynamics 365 Guides issue. To learn about the schedule for changes to these platforms, see the following articles:

- [Released versions of Microsoft Dataverse](/dynamics365/released-versions/microsoft-dataverse)
- [Released versions of Dynamics 365 Core Service Scheduling](/dynamics365/released-versions/dynamics365-css)
- [Update history for Microsoft Teams app version (Public Cloud and GCC)](/officeupdates/teams-app-versioning)

## I can't install the Dynamics 365 Guides solution because I can't find it in the Power Platform admin center

If you previously set up a Dataverse environment instance in a different region than your tenant's default region, the Dynamics 365 Guides model-driven app will not be available to install. You must first [contact Microsoft support](https://support.serviceshub.microsoft.com/supportforbusiness) and ask to make your tenant into a multi-geo tenant for Power Platform.  

## I'm connected through a proxy or VPN and can't sign in to Dynamics 365 Guides. What can I do?

If you're having problems signing in to or using Dynamics 365 Guides, it may be that your network isn't configured correctly. 

[Learn how to configure a VPN or proxy for Dynamics 365 Guides](admin-deployment-playbook.md#vpn-or-proxy-configuration).

## Does Dynamics 365 Guides support HoloLens (1st gen)?

HoloLens (1st gen) has entered Long Term Servicing State and is no longer supported on the latest versions of Dynamics 365 Guides. Customers on HoloLens (1st gen) can continue using the last supported app version (600.2103.19001) released on April 1, 2021. This version of the app is compatible with all 500 solution versions up to and including 600.0.0.1, also released on April 1, 2021. To continue using HoloLens (1st gen), existing customers should not upgrade to a solution version later than 600.0.0.1. Solution version 600.0.0.1 is no longer available for download for new HoloLens 1 customers.

## Why are there two apps?

Dynamics 365 Guides includes two applications, which enable authors and operators to use the right device for the right task in their workflows:

- **PC authoring app.** Authors use the PC app to add content and to create and structure their guide. These tasks are fast and efficient on a PC.

- **[!include[pn-hololens](../includes/pn-hololens.md)] app.** This app includes modes for authoring and operating.

    - **Authors** use the HoloLens app to anchor their guides and place holograms where they belong in the real world.

    - **Operators** use the HoloLens app to access the step-by-step holographic work instructions. Operators never need to use the PC app. 

If you plan to author guides, you'll need to use both apps. If not, you'll only need the [!include[pn-hololens](../includes/pn-hololens.md)] app.

## What languages is Dynamics 365 Guides available in?

See a [list of product availability by language](https://dynamics.microsoft.com/en-us/availability-reports/languagereport/). 

Dynamics 365 Guides is listed in the hierarchy under **Dynamics 365**>**Operations Apps**. 

## Why do I see the Step content failed to load message in the HoloLens app?

If the amount and complexity of content added to a step will result in a poor experience for the operators of the guide, Dynamics 365 Guides displays a series of warnings. When the complexity reaches a certain limit, you'll see the following message.

![Screenshot of Step content failed to load message.](media/step-content-failed-load.jpg "Screenshot of Step content failed to load message")

You can't place any additional 3D models at this point. If a model was previously placed in the world, it will be represented as an exclamation point icon to authors and operators. [Learn more about warnings and how to reduce step complexity](hololens-app-place-holograms.md)

## Is there an out-of-the-box integration with Dynamics 365 Field Service?

Yes, [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] integration was added in version 104.1907.19001.

## How do I stream my HoloLens view to a PC using Miracast?

The Connect app for wireless projection using Miracast is no longer installed by default on the PC, but is available as an optional feature. To install the app on the PC, select **Settings** > **Apps** > **Optional features** > **Add a feature**, and then install the Wireless Display app. 

The Connect app is automatically installed by default on the HoloLens. To initiate sharing from the HoloLens:

From the OS start menu, select **Cast screen** :::image type="icon" source="media/hololens-cast-screen.png":::.

## The solution installation or update fails repeatedly

To update the solution, you must have the [System Administrator](/power-platform/admin/database-security) role AND you must have a [Power Apps license](/power-platform/admin/signup-question-and-answer) (or a license like a [Dynamics 365 Guides license](setup-step-one.md) that includes a Power Apps license). 

![Dynamics 365 Guides license selected.](media/dynamics-365-guides-license.PNG "Dynamics 365 Guides license selected")

When you have a Power Apps license, the Access Mode security property is set to Read-Write, which is required for updating the solution. 

## I don't see my Dynamics 365 Guides environment even though I have a valid Dynamics 365 Guides license. What should I do? 

You might have installed Dynamics 365 Guides on a trial environment that has expired. Trial environments have their own life cycle, independent of the Dynamics 365 Guides license. You can go to [Power Platform admin center](https://admin.powerplatform.microsoft.com/environments), select your trial environment, and switch it to a production environment.

## How do I limit users to a particular Dynamics 365 instance?

You can limit user access to instances by using security groups that are managed in the Microsoft 365 admin center. For more information, see [Restrict access to an instance in Dynamics 365 Guides by using security groups](admin-security.md) and [Control user access to instances: security groups and licenses](/dynamics365/admin/add-instance-subscription#control-user-access-to-instances-security-groups-and-licenses).

## I get an error message when I try to sign in to the PC app or [!include[pn-hololens](../includes/pn-hololens.md)] app

The [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution package (which includes the built-in library of 3D content) needs to be installed on your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account. Every user must also have a license to use the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] product. If your organization is already subscribed to [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], you or your admin can easily provide access to the apps. For more information, [see the Setup topic](setup.md).

## Where is the data stored, and who has access to it?

The data is stored in Microsoft Dataverse in the tenant that you have admin privileges to. Please sign in to [!include[pn-dyn-365](../includes/pn-dyn-365.md)] using the credentials created during the sign-up process. For more information, [see the Setup topic](setup.md). 

## What file formats are supported?

For a list of formats that are supported for 3D content, images, and videos, see [Supported file formats](pc-app-supported-file-formats.md).

## Will I lose any data if I close an app inadvertently while authoring?

Both apps automatically save your edits as you author a guide. After you're done editing, we recommend pausing for a couple seconds before closing the app to make sure the app has time to sync with the server.

Note that in the [!include[pn-hololens](../includes/pn-hololens.md)] application, if you leave the app, it goes on standby (doesn't close). When you select the app tile, you'll return to where you were before, and no changes will be lost.

## What keyboard shortcuts are available in the PC authoring app?

For a list of keyboard shortcuts, see [Keyboard shortcuts for the PC app](keyboard-shortcuts-pc-app.md).

## What does the Save button with the refresh icon mean? How does Save work?

The Autosave functionality enables authors to synchronize their changes across the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps when editing a guide at the same time in both apps. Edits are automatically saved and synced to the server every few seconds. The apps will also refresh automatically when they detect any changes made to the guide from another device. You can also select the **Save** button at any time if you want to be sure your edits are saved.

## I see this message: "Guide out of sync… refreshing" with a loading spinner. What's going on?

This message is displayed when you or another user are editing the same guide on separate devices. The guide is automatically saved on the other device first, then updated on the server. When the current device learns of the update, it reloads the latest version of the guide from the server.

## I see this message: "Save failed." What does this mean?

The PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps save your changes to the server two seconds after each change is made. If any of these save attempts fail, you'll see this notification.

This might occur if you have a poor internet connection or if the server is down. The notification should go away automatically after the server connection is restored. However, if this message doesn't go away, we suggest that you not make more edits during that session, because your edits might be lost. Check the internet connection on your device or speak with your administrator to see whether there are any connectivity issues.

## Can I add more than eight 3D models to a step?

There are only eight **3D parts** boxes in the bin, which limits the variety of 3D models you can add to a single step. When placing holograms on the [!include[pn-hololens](../includes/pn-hololens.md)], you can, however, place an unlimited number from the bin. For example, you can add up to eight different 3D models (arrows, boxes, nuts, drills, and so on) to the bin, but you can place as many arrows, boxes, nuts, and drills from each **3D Parts** box that you want when in [!include[pn-hololens](../includes/pn-hololens.md)]. To do this, either tap the asset bins to spawn 3D models or go to a 3D model's **Edit** menu and select **Duplicate**.

## I see a triangle-shaped hazard sign when I load a step. What does that mean?

The hazard sign is a placeholder for 3D models, videos, or images that can't be successfully loaded in the [!include[pn-hololens](../includes/pn-hololens.md)] app. Possible reasons for this:

- This might occur due to intermittent connectivity issues or because the file is too large. If you see this, please relaunch the [!include[pn-hololens](../includes/pn-hololens.md)] app. If this doesn't fix the problem, launch the PC app, find the file in question, and open it in preview mode. If the preview loads, reinstall the [!include[pn-hololens](../includes/pn-hololens.md)] app and try launching the guide again. 

- If you can't find the file in the PC app library, the reference (entity) to the 3D model/video/image is broken. Please upload the file again and re-author the guide.

- If the file exists in the library but the preview doesn't load, there's a problem with the file information in [!include[pn-dyn-365](../includes/pn-dyn-365.md)]. Please upload the file again, and then edit the guide to refer to this new asset wherever applicable.

## Why does the HoloLens app require permissions to launch?

The HoloLens app includes advanced features that rely on eye-tracking, voice, camera, and movement to function properly. For example, you need eye tracking to access the Main menu. [Learn more about the permissions required to use the HoloLens app](hololens-permissions.md)  

## Why can't I make a video call?

If you're using Dynamics 365 Guides version 7.0 or later and you can’t make a video call, it could be because:

-	Your admin has [disabled the option directly from the Guides web portal](admin-enable-calls.md). 

-	The appropriate Microsoft Teams license has not been assigned to you. [Learn more about licensing requirements](requirements.md).

-	You're currently offline and need to reconnect to the internet.

## See also

[Known Issues in Dynamics 365 Guides](known-issues.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
