---
title: Restrict the ability for Dynamics 365 Remote Assist users on HoloLens from signing out of the app
author: prashantyvr
description: Learn how to restrict users of Microsoft Dynamics 365 Remote Assist from signing out of the app. 
ms.author: prashan
ms.date: 06/07/2024
ms.topic: article
ms.reviewer: v-wendysmith
---

# Restrict Dynamics 365 Remote Assist users on HoloLens from signing out of the app

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Microsoft Dynamics 365 Remote Assist users on HoloLens from signing out. This restriction prevents them from changing user accounts. You can do this by [setting up HoloLens as a kiosk](/hololens/hololens-kiosk?tabs=uisak%2Cautologon). When you set up HoloLens in kiosk mode, Dynamics 365 Remote Assist automatically prevents users from signing out of the app. You can also use kiosk mode to show selected apps in the **Start** menu. 

**HoloLens users must be on OS version 22H1 (Spring 2022 release) or later to use kiosk mode.**

> [!NOTE]
> At this time, if you configure HoloLens for multiple apps kiosk mode, the **Sign out** button in Dynamics 365 Remote Assist isn't disabled. The **Sign out** button is disabled if you configure HoloLens for single app kiosk mode. 

## See also

- [Set up HoloLens as a kiosk](/hololens/hololens-kiosk?tabs=uisak%2Cautologon)
- [Overview of restricting capabilities in Dynamics 365 Remote Assist](restricted-mode-overview.md)
- [Restrict calling and the ability to search and access contacts](restricted-mode-calling.md)
- [Restrict the ability to access OneDrive files](restricted-mode-files.md)
- [Restrict the ability to access asset records](restricted-mode-assets.md)
