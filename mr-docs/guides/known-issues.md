---
author: davepinch
description: Known issues with Dynamics 365 Guides (general issues)
ms.author: davepinch
ms.date: 08/08/2023
ms.topic: article
title: Known issues with Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Known issues with Microsoft Dynamics 365 Guides

## I can't open a guide because it's corrupted

In very rare cases, you might find that a guide has become corrupted. This is most commonly associated with guides that were [shared with authors](admin-share-guide.md) in the time period from September 2021 to December 2021. If you open a corrupted guide in the PC app, the following message appears. 

![Screenshot of message that appears when a guide is corrupted.](media/corrupted-guide-message.jpg "Screenshot of message that appears when a guide is corrupted")

[Learn how to fix a corrupted guide](corrupted-guide.md)

## I don't see any guides in the Guides list

If you don't see any guides, either your internet connection is unstable, or you might have signed in to an environment that doesn't have any guides. First, check your internet connection. If you're connected, try to sign in again, and make sure that you sign in to the environment that has the guides that you're looking for. If you still don't see any guides, contact your admin.

## The Create account link doesn't work when I try to use a new account to sign in

When you sign in with a brand new account on the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps, there's a link to create a new account:

![Sign-in screen.](media/sign-in-screen.PNG "Sign-in screen")
 
Don't use this link to create an account–it doesn't work.

## I can't see guides that I created or guides that my teammates created

If you don't see any guides, either your internet connection is unstable, or you might have signed in to an environment that doesn't have any guides. First, check your internet connection. If you're connected, try signing in again, but this time make sure you sign into the environment that has the guides you were looking for. If you still don't see any guides, contact your administrator.

## Text wrapping on the PC and in HoloLens might differ in rare cases

In rare cases, you might notice that text is wrapped in the Step card view in [!include[pn-hololens](../includes/pn-hololens.md)] but not on the PC. This issue occurs because, for the sake of readability, [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] renders fonts at different sizes on the PC and in [!include[pn-hololens](../includes/pn-hololens.md)], and different widths of characters might cause them to go to the next line. To ensure that this issue doesn't affect the operator experience, validate the text for all steps in the [!include[pn-hololens](../includes/pn-hololens.md)] app before you share your guides with operators.

## In the Guides app on HoloLens, moving holograms becomes less responsive

You can reset the app on HoloLens.

On HoloLens, go to **HoloLens Settings** > **Apps** > **Dynamics 365 Guides** > **Advanced Options** > **Reset** and reset the app. This action restores responsiveness when authoring hologram positions.

## I have an issue that isn't listed in these troubleshooting steps

Contact customer service: [Get support for your Dynamics 365 product](/dynamics365/get-started/support/). This page can also be found by signing in to your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account and selecting the **Support** link.

## See also

- [Known issues with the PC app](known-issues-pc-app.md)
- [Known issues with the HoloLens app](known-issues-hololens-app.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
