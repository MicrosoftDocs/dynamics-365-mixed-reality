---
author: Mamaylya
description: Learn about how HoloLens (first gen) works with and Dynamics 365 Guides
ms.author: mamaylya
ms.date: 11/08/2021
ms.topic: article
title: Use HoloLens (first gen) devices with Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Use HoloLens (first gen) devices with Dynamics 365 Guides

HoloLens (first gen) has entered Long Term Service State for Dynamics 365 Guides. This article accumulates all documentation related to using HoloLens (first gen) devices with Dynamics 365 Guides.



## Calibrate your HoloLens 1 device

> [!IMPORTANT]
> In Dynamics 365 Guides version 502.2011.28001 (December 8, 2020 release) and later, HoloLens operating system version 10.0.17134 (Redstone 4) is no longer supported. This version of the operating system is used only on HoloLens 1. HoloLens 1 customers must upgrade to HoloLens version 10.0.17763 or later to continue to receive the latest updates. Work with your IT admin to update your HoloLens operating system. If you choose not to upgrade, you can continue to use the current version of Dynamics 365 Guides that is already installed on the device. However, HoloLens version 10.0.17763 or later is required to install Dynamics 365 Guides on any new or refactored HoloLens 1 device. 

1. Use the bloom gesture to open the **Start** menu.

2. Air tap **Calibration**.

    ![Calibration button.](media/hololens-calibration.PNG "Calibration button")

3. Follow the instructions on your [!include[pn-hololens](../includes/pn-hololens.md)].

All users must do this calibration after they sign in to the device. If HoloLens is running Windows Holographic for Business edition, the IPD settings are saved on the device. When you sign in to the same HoloLens, your IPD settings are automatically applied, even after you switch users; you don't have to recalibrate the device. However, if HoloLens is running Windows Holographic edition, user settings aren't saved because this version of the operating system is designed for a single user. So you must recalibrate the device whenever you switch users.

To determine which version of the operating system you're using on [!include[pn-hololens](../includes/pn-hololens.md)], follow these steps.

1. Use the bloom gesture to open the **Start** menu.

2. Air tap **Settings \> System**.

3. Air tap **About**.
