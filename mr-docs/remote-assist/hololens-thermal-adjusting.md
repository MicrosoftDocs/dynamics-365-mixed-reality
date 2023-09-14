---
title: How Dynamics 365 Remote Assist automatically adjusts HoloLens temperature if the device overheats
author: davepinch
description: Learn how Dynamics 365 Remote Assist automatically adjusts HoloLens temperature by reducing outgoing video quality if the device overheats
ms.author: davepinch
ms.date: 06/10/2022
ms.topic: article
ms.reviewer: v-wendysmith
---

# How Dynamics 365 Remote Assist automatically adjusts HoloLens temperature if the device overheats

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

If you're on a longer call in Microsoft Dynamics 365 Remote Assist for HoloLens, the HoloLens device can become hot if it's using 
several device capabilities at the same time (for example, multiple cameras, Mixed Reality Capture, and Wi-Fi). To extend the length of the call and keep the device 
from overheating, Dynamics 365 Remote Assist gradually reduces outgoing video quality (resolution and frame rate). If this happens, you'll see a series of messages to let you know how and why outgoing video quality is being adjusted. 

> [!IMPORTANT]
> You must use HoloLens OS version 22H1 (Spring 2022 release) or later to use this feature. Also, the Dynamics 365 Remote Assist application must be in the foreground (have the focus) to adjust to temperature changes.  

The first warning message tells you that HoloLens is heating up and that outgoing video quality has been reduced.

![Screenshot of HoloLens message showing that device is heating up.](media/hololens-thermal-warning-1.jpg "Screenshot of HoloLens message showing device is heating up")

If the device continues to heat up, you'll see a warning that the device is continuing to reach critical temperatures and that outgoing video quality has been further reduced.

![Screenshot of HoloLens message showing that device is continuing to heat up.](media/hololens-thermal-warning-2.jpg "Screenshot of HoloLens message showing device is continuing to heat up")

If the device reaches a critical temperature, you'll see a warning that outgoing video has been disabled. 

![Screenshot of HoloLens message showing device has reached critical temperature.](media/hololens-thermal-warning-3.jpg "Screenshot of HoloLens message showing device has reached critical temperature")

If you attempt to activate video after it has been disabled, you'll see a message that says outgoing video is unavailable. 

![Screenshot of HoloLens message showing device has been disabled.](media/hololens-thermal-warning-4.jpg "Screenshot of HoloLens message showing device has been disabled")

When the device returns to an optimal operating temperature, you'll see a message that says outgoing video quality has been restored.

![Screenshot of HoloLens message showing outgoing video has been restored.](media/hololens-thermal-restore.jpg "Screenshot of HoloLens message showing outgoing video has been restored")

If you had video turned on before it was disabled, the video will automatically be turned back on. If you had video turned off before it was disabled, it will remain off but you can turn it back on. 

