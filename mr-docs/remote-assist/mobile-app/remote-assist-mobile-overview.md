---
title: Dynamics 365 Remote Assist mobile overview
author: amaraanigbo
description: Get an overview of the Dynamics 365 Remote Assist mobile app capabilities.
ms.author: soanigbo
ms.date: 10/01/2020
ms.topic: overview
ms.reviewer: v-bholmes
---

# Dynamics 365 Remote Assist mobile overview

Dynamics 365 Remote Assist enables technicians with mobile devices to connect with a remote collaborator on Dynamics 365 Remote Assist mobile or Microsoft Teams (desktop or mobile). Using live video calling, mixed-reality annotations, and high-resolution snapshots, they can share what they see with the remote collaborator to troubleshoot problems together, faster.

![Simulated image of a technician using Dynamics 365 Remote Assist mobile to annotate their environment on a call.](./media/ram-overview.png "Dynamics 365 Remote Assist mobile Overview")

Dynamics 365 Remote Assist mobile is beneficial in scenarios where technicians may need physical access to confined or hard-to-reach spaces, or access to other mobile apps that are part of their organizations' workflows. With the availability and familiarity with mobile devices, technicians can use Dynamics 365 Remote Assist mobile during repairs and inspections with ease. Furthermore, Dynamics 365 Remote Assist mobile allows for easier broad-scale deployment in organizations.

Dynamics 365 Remote Assist is available on [Android phones and tablets with ARCore support](https://developers.google.com/ar/discover/supported-devices) and [iOS iPhones and iPads with ARKit support](https://developers.google.com/ar/discover/supported-devices#ios). Additionally, Dynamics 365 Remote Assist is available on mobile devices **without** ARCore or ARKit support, too! Visit our [documentation on product requirements](../requirements.md) to learn more.

## Features

- One-to-one and group video calling.
- Add mixed-reality annotations in space.
- Use asset capture in offline scenarios to annotate, capture, and visualize images and videos of assets and store them in Microsoft Dataverse. 
- Annotate on a 2D image capture, or snapshot, of the space during a call.
- Send and receive messages, in-call snapshots, and files through text chat.
- Capture session history through call recordings.
- Annotate and share in-call snapshots in low-bandwidth scenarios.
- Availability on mobile devices without augmented reality (AR) support.
- Integration with Microsoft Dynamics 365 for Field Service.
   - Ability to link call history, in-call snapshots, and files shared during a Dynamics 365 Remote Assist mobile call to an associated Dynamics 365 Field Service work order.
   - Ability to start a call to a remote collaborator from the Dynamics 365 Field Service mobile app to the Dynamics 365 Remote Assist mobile app.

## Microsoft Intune support

Dynamics 365 Remote Assist mobile for iOS and Android supports Microsoft Intune's app protection policies. These policies ensure that data remains safe and contained on the device through Intune policies.  

![Graphic showing Intune controls.](./media/RAM_IntuneControls.png)

[Learn how to create an app configuration policy for Android devices](intune.md)

## Videos

- [Watch a technician use Dynamics 365 Remote Assist mobile on-site](https://www.youtube.com/watch?v=J-C6GE2gFYw&t=27s).
- [Watch a live demo of Dynamics 365 Remote Assist mobile in action, from signing in to ending the call](https://www.youtube.com/watch?v=DQJWsCDNpb4&t=1s).

## See also

- [Try Dynamics 365 Remote Assist mobile for free](../try-remote-assist.md)
- [Buy a Dynamics 365 Remote Assist license](../buy-remote-assist.md)
- [Deploy Dynamics 365 Remote Assist](../deploy-remote-assist.md)
- [How-to videos for Dynamics 365 Remote Assist mobile](../videos.md)
- [Use Microsoft Intune to create an app configuration policy for Android devices](intune.md) 
- [FAQ](/dynamics365/mixed-reality/remote-assist/faq#using-remote-assist-on-mobile)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
