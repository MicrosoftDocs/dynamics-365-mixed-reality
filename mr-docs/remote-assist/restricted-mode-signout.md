---
title: Restrict the ability for Dynamics 365 Remote Assist users on HoloLens from signing out of the app
author: amaraanigbo
description: Learn how to restrict users of Microsoft Dynamics 365 Remote Assist from signing out of the app. 
ms.author: soanigbo
ms.date: 04/22/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Restrict Dynamics 365 Remote Assist users on HoloLens from signing out of the app

If you [have a scenario where you need to protect your company information](restricted-mode-overview.md), you can restrict the ability for Microsoft Dynamics 365 Remote Assist users on HoloLens from signing out. This restricts their ability to change user accounts. You can do this by [setting up HoloLens in kiosk mode](https://docs.microsoft.com/hololens/hololens-kiosk?tabs=uisak%2Cautologon). When you set up HoloLens in kiosk mode, Dynamics 365 Remote Assist automatically prevents users from signing out of the app. You can also use kiosk mode to show just selected apps in the **Start** menu. 

**HoloLens users must be on OS version 22H1 (Spring 2022 release) or later to use kiosk mode.** You can't use kiosk mode to restrict users of the mobile app from signing out of the app. 

> [!NOTE]
> At this time, if you configure HoloLens for multiple app kiosk mode, the **Sign out** button in Dynamics 365 Remote Assist is not disabled. The **Sign out** button is disabled if you configure HoloLens for single app kiosk mode. 

## See also

- [Set up HoloLens in kiosk mode](https://docs.microsoft.com/hololens/hololens-kiosk?tabs=uisak%2Cautologon)
- [Overview of restricting capabilities in Dynamics 365 Remote Assist](restricted-mode-overview.md)
- [Restrict calling and the ability to search and access contacts](restricted-mode-calling.md)
- [Restrict the ability to access OneDrive files](restricted-mode-files.md)
- [Restrict the ability to access asset records](restricted-mode-assets.md)
