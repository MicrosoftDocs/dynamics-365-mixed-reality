---
author: Mamaylya
description: Learn about things you can do to improve positional precision of holograms in Dynamics 365 Guides
ms.author: mamaylya
ms.date: 11/03/2020
ms.service: crm-online
ms.topic: article
title: Improve positional accuracy of holograms in Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Effect of calibration, pre-scanning, and environment on positional precision of holograms in Dynamics 365 Guides

This article describes several things that you can do to improve positional precision of holograms in Microsoft Dynamics 365 Guides.

> [!IMPORTANT]
> In addition to the suggestions in this article, make sure to also review the following articles:
>
> - [Anchor types/placement and their effect on positional precision of holograms](pc-app-anchor-types-placement-precision.md)
> - [Best practices for QR code anchors](pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors)
> - [Best practices for circular code anchors](pc-app-anchor-circular-code.md#best-practices-for-circular-code-anchors)
> - [Best practices for holographic anchors](pc-app-anchor-holographic.md#best-practices-for-holographic-anchors)

## Calibrate the device to the operator's interpupillary distance (IPD)

IPD is the distance between the center of the user's pupils. Because different users might have different IPDs, it's crucial that the appropriate IPD is set, so that HoloLens can adapt its display. An incorrect IPD setting can cause inaccurate perception of hologram position. 

To calibrate device eye-tracking and IPD on HoloLens 2, make sure to use the eye calibration app when prompted. This will not only calibrate IPD but will also enable HoloLens 2 to auto-correct hologram position in case the device moves on the operator's head. You can also [manually calibrate the device at any time](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/guides/operator-calibrate-hl2) on HoloLens 1 or HoloLens 2.

## Pre-scan the environment

HoloLens actively scans its environment for visible features to map its surroundings. This scan occurs whenever the device is turned on and a user is signed in. It occurs whether the user is in the HoloLens shell (the state when no immersive apps are launched) or running apps. HoloLens constantly improves the accuracy of these maps as it scans the environment from different viewpoints and stores the maps on the device. Holograms are placed in relation to these maps. The more accurate the map, the more accurate the hologram placement.

Before an operator uses Dynamics 365 Guides on a HoloLens that hasn't been used in a particular environment, it's helpful for the author to put on the HoloLens, sign in to the device, and walk around the space where hologram instructions have been placed or will be placed. This process is called "pre-scanning" because it's done before running Dynamics 365 Guides. You only need to complete this process once for each environment, because HoloLens stores the maps that it creates on the device and remembers the spaces that it has scanned. 

Although the author can do this step from the HoloLens shell, we recommend hiding the **Start** menu, so the author can see the space as they walk around. Walking at a leisurely pace while slowly looking up and down and air tapping gives the device an opportunity to find features and construct accurate maps. The author can see the reconstructed 3D map the device has already built and identify areas that might lack mapping. 

> [!NOTE] 
> To clear the maps and all registered holograms from the device, go to **Settings** > **System** > **Holograms** > **Remove all holograms**.

Authors should pre-scan the environment in representative light conditions and space configurations.

## Choose an environment with a high number of visible features

HoloLens builds maps of its surroundings and tracks its position and hologram position based on visible features (high contrast point and corners) in the environment. If the space in which HoloLens is operating has a low number of visible features (mostly white walls for example), or very repetitive patterns (textured surfaces), this will impact hologram position and stability as HoloLens won’t be able to properly identify and track uniquely specific points in the environment.

## Avoid reflective, dark, or featureless surfaces

Environments that include very reflective surfaces (mirrors), dark surfaces, or featureless surfaces (cleanrooms), negatively affect the ability of HoloLens to recognize the space. If HoloLens can't correctly recognize the space, hologram position and stability are affected in turn.

## Avoid unstable lighting conditions

Lighting conditions have an impact on how HoloLens perceives the environment and recognizes the space. Environments with unstable lighting conditions are prone to hologram instability. If the light changes significantly, HoloLens might consider the space as a new environment and build a new map for it. Previously visible features might be invisible and features that weren’t visible might be visible. 

## HoloLens 1 only: Make sure to wear the device in a consistent way

HoloLens uses a novel display technology to project holograms in the operator's field of view. On HoloLens 1, the way that operators wear a device on their head has a huge impact on the perceived position of the holograms. The best way to understand this is to adjust the device positioning while aligning holograms to their physical counterparts in Dynamics 365 Guides. Notice how the alignment of holograms is affected when you shift the device left and right, up and down, or forward and backward. Operators should wear the device in a consistent way, and they should understand that subtle shifts in device positioning might not feel different but can cause significant changes in perceived hologram locations. On HoloLens 2, issues with device positioning are addressed through eye tracking.

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Anchoring overview|[Overview of anchoring a guide](pc-app-anchor.md)|
|Creating types of anchors|[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|Hologram precision|[Effect of anchor types/placement](pc-app-anchor-types-placement-precision.md)|
|HoloLens app for authors|[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)|
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)
