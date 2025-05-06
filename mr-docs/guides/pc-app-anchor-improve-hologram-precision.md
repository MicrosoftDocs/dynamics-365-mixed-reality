---
author: prashantyvr
description: Learn about things you can do to improve positional precision of holograms in Dynamics 365 Guides
ms.author: prashan
ms.date: 02/27/2024
ms.topic: article
title: Effect of calibration, prescanning, and environment on positional precision of holograms in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Effect of calibration, prescanning, and environment on positional precision of holograms in Dynamics 365 Guides

This article describes several things that you can do to improve positional precision of holograms in Microsoft Dynamics 365 Guides.

> [!IMPORTANT]
> In addition to the suggestions in this article, make sure to review the following articles:
>
> - [Anchor types/placement and their effect on positional precision of holograms](pc-app-anchor-types-placement-precision.md)
> - [Best practices for QR code anchors](pc-app-anchor-qr-best-practices.md)
> - [Best practices for circular code anchors](pc-app-anchor-circular-best-practices.md)
> - [Best practices for holographic anchors](pc-app-anchor-holographic-best-practices.md)

## Calibrate the device to the user's interpupillary distance (IPD)

IPD is the distance between the center of the user's pupils. Because different users might have different IPDs, it's crucial that the appropriate IPD is set, so that HoloLens can adapt its display. An incorrect IPD setting can cause inaccurate perception of hologram position. 

To calibrate device eye-tracking and IPD on HoloLens 2, make sure to use the eye calibration app when prompted. This app helps you calibrate IPD but also enables HoloLens 2 to autocorrect hologram position in case the device moves on the operator's head. You can also [manually calibrate the device at any time](./operator-calibrate-hl2.md).

## Prescan the environment

HoloLens actively scans its environment for visible features to map its surroundings. This scan occurs whenever the device is turned on and a user is signed in. It occurs whether the user is in the HoloLens shell (the state when no immersive apps are launched) or running apps. HoloLens constantly improves the accuracy of these maps as it scans the environment from different viewpoints and stores the maps on the device. Holograms are placed in relation to these maps. The more accurate the map, the more accurate the hologram placement.

Before an operator uses Dynamics 365 Guides on a HoloLens that hasn't been used in a particular environment, the author should put on the HoloLens, sign in to the device, and walk around the space where hologram instructions have been placed. This process is called "prescanning" because it's done before running Dynamics 365 Guides. The author only needs to complete this process once for each environment, because HoloLens stores the maps that it creates on the device and remembers the spaces that it has scanned. 

Although the author can do this step from the HoloLens shell, we recommend hiding the **Start** menu, so the author can see the space as they walk around. Walking at a leisurely pace while slowly looking up and down and air tapping gives the device an opportunity to find features and construct accurate maps. The author can see the reconstructed 3D map the device has already built and identify areas that might lack mapping. 

> [!NOTE] 
> To clear the maps and all registered holograms from the device, go to **Settings** > **System** > **Holograms** > **Remove all holograms**.

Authors should prescan the environment in representative light conditions and space configurations.

## Choose an environment with a high number of visible features

HoloLens builds maps of its surroundings and tracks its position and hologram position based on visible features (high contrast points and corners) in the environment. If the space in which HoloLens is operating has a low number of visible features (mostly white walls for example), or repetitive patterns (textured surfaces), impacts hologram position and stability. HoloLens can't properly identify and track uniquely specific points in the environment.

## Avoid reflective, dark, or featureless surfaces

Environments that include reflective surfaces (mirrors), dark surfaces, or featureless surfaces (cleanrooms), negatively affect the ability of HoloLens to recognize the space. If HoloLens can't correctly recognize the space, hologram position and stability are affected in turn.

## Avoid unstable lighting conditions

Lighting conditions impacts how HoloLens perceives the environment and recognizes the space. Environments with unstable lighting conditions are prone to hologram instability. If the light changes significantly, HoloLens might consider the space as a new environment and build a new map for it. Previously visible features might be invisible and features that weren’t visible might be visible. 

## Next steps

- [Overview of anchoring a guide](pc-app-anchor.md)
- [Create an object anchor  in the PC app](pc-app-anchor-object.md)
- [Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)
- [Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)
- [Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
