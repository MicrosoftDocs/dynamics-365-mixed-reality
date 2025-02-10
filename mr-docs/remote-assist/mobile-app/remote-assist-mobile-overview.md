---
title: Dynamics 365 Remote Assist mobile overview
description: Discover the features and functions of Dynamics 365 Remote Assist mobile app.
author: prashantyvr
ms.author: prashan
ms.date: 02/10/2025
ms.topic: overview
ms.reviewer: v-wendysmith
---

# Dynamics 365 Remote Assist mobile overview

[!INCLUDE [ra-mobile-deprecate-include](../../includes/ra-mobile-deprecate.md)]

Microsoft Dynamics 365 Remote Assist enables technicians with mobile devices to connect with a remote collaborator on Dynamics 365 Remote Assist mobile or Microsoft Teams (desktop or mobile). Using live video calling, mixed-reality annotations, and high-resolution snapshots, they can share what they see with the remote collaborator to troubleshoot problems together, faster.

![Simulated image of a technician using Dynamics 365 Remote Assist mobile to annotate their environment on a call.](./media/ram-overview.png "Dynamics 365 Remote Assist mobile Overview")

Dynamics 365 Remote Assist is available on [Android phones and tablets with ARCore support](https://developers.google.com/ar/discover/supported-devices) and [iOS iPhones and iPads with ARKit support](https://developers.google.com/ar/discover/supported-devices#ios). Additionally, Dynamics 365 Remote Assist is available on mobile devices **without** ARCore or ARKit support. To learn more, visit our [documentation on product requirements](../requirements.md).

## Features

Compare what features are available on Microsoft Teams mobile versus Remote Assist mobile.

|Features|Available in Teams mobile|Available in Remote Assist mobile|
|:----|:----|:----|
|One-to-one and group video calling|Yes|Yes|
|Add mixed-reality annotations in space|Yes|Yes|
|Use asset capture in offline scenarios to annotate, capture, and visualize images and videos of assets and store them in Microsoft Dataverse|No|Yes|
|Annotate on a 2D image capture, or snapshot, of the space during a call|Yes|Yes|
|Send and receive messages, in-call snapshots, and files through text chat|Yes|Yes|
|Capture session history through call recordings|Yes|Yes|
|Annotate and share in-call screenshots in low-bandwidth scenarios|Yes|Yes|
|Availability on mobile devices without augmented reality (AR) support|Yes|Yes|
|Integration with Microsoft Dynamics 365 for Field Service: Ability to link call history, in-call snapshots, and files shared during a Remote Assist mobile call to an associated Dynamics 365 Field Service work order. |No|Yes|
|Integration with Microsoft Dynamics 365 for Field Service: Ability to start a call to a remote collaborator from the Dynamics 365 Field Service mobile app in Teams.|Yes|Yes|

## Microsoft Intune support

Dynamics 365 Remote Assist mobile for iOS and Android supports Microsoft Intune's app protection policies. These policies ensure that data remains safe and contained on the device through Intune policies.  

![Graphic showing Intune controls.](./media/RAM_IntuneControls.png)

[Learn how to create an app configuration policy for Android devices.](intune.md)

## Videos

- [Watch a technician use Dynamics 365 Remote Assist mobile on-site](https://www.youtube.com/watch?v=J-C6GE2gFYw&t=27s)
- [Watch a live demo of Dynamics 365 Remote Assist mobile, from signing in to ending the call](https://www.youtube.com/watch?v=DQJWsCDNpb4&t=1s)

## See also

- [Buy a Dynamics 365 Remote Assist subscription](../buy-remote-assist.md)
- [Deploy Dynamics 365 Remote Assist](../deploy-remote-assist.md)
- [How-to videos for Dynamics 365 Remote Assist mobile](../videos.md)
- [FAQ](faq-mobile.md)

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
