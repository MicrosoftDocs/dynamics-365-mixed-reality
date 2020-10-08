---
author: Mamaylya
description: Learn about various factors that can affect positional consistency when anchoring a guide with the Dynamics 365 Guides PC app
ms.author: mamaylya
ms.date: 10/01/2020
ms.service: crm-online
ms.topic: article
title: Things that can affect positional consistency when anchoring a guide with the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Things that can affect positional consistency when anchoring a guide with the Dynamics 365 Guides PC app

The following things can affect positional consistency when anchoring a guide with the Microsoft [Dynamics 365 Guides PC app](pc-app-anchor.md).

> [!IMPORTANT]
> In addition to the suggestions included in this article, make sure to review best practices for each type of anchor:
>
> - [Best practices for QR code anchors](pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors)
> - [Best practices for circular code anchors](pc-app-anchor-circular-code.md#best-practices-for-circular-code-anchors)
> - [Best practices for holographic anchors](pc-app-anchor-holographic.md#best-practices-for-holographic-anchors)

## Eye calibration and Interpupillary Distance (IPD) setting

IPD is the distance between the center of the user's pupils. Because different users might have different IPDs, it's crucial that the appropriate IPD is set, so that HoloLens can adapt its display. An incorrect IPD setting can cause inaccurate perception of hologram position. 

- To calibrate the device eye-tracking and IPD on HoloLens 2, make sure to use the eye calibration app when prompted. This will not only calibrate IPD but will also enable HoloLens 2 to auto-correct hologram position in case the device moves on the operator's head. If you're not prompted to use the eye calibration app, [you can start manually calibrate the device](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/guides/operator-calibrate-hl2).

- To calibrate IPD on HoloLens 1, use the HoloLens Calibration app.

## Pre-scanning the environment

HoloLens actively scans its environment for visible features to map its surroundings. This scan occurs whenever the device is turned on and a user is signed in. It occurs regardless of whether you're in the HoloLens shell or running apps. HoloLens constantly improves the accuracy of these maps as it scans the environment from different viewpoints and stores the maps on the device. Holograms are placed in relation to these maps. The more accurate the map, the more accurate the hologram placement.

Before using Dynamics 365 Guides on a HoloLens that hasn't been used in a particular environment, have the operator put on the HoloLens, sign in to the device, and walk around the space where hologram instructions have been placed or will be placed. Although the operator can do this step from the HoloLens shell, we recommend hiding the **Start** menu, so the operator can see the space as they walk around. By walking at a leisurely pace while slowly looking up and down, the operator gives the device an opportunity to find features and construct accurate maps.

This process is called "pre-scanning," because it's done before running Dynamics 365 Guides. You only need to complete this process once for each environment, because HoloLens stores the maps that it creates on the device and remembers the spaces that it has scanned. 

By looking around and air tapping, you will be able to see the reconstructed 3D map the device has already built, giving you the opportunity to identify areas that might lack mapping. You always have the option to clear the maps and all registered holograms from the device by going to **Settings** > **System** > **Holograms** > **Remove all holograms**.

## Surface type

Environments that include very reflective surfaces (mirrors), dark surfaces, or featureless surfaces (cleanrooms), negatively affect the ability of HoloLens to recognize the space. If HoloLens can't correctly recognize the space, hologram position and stability are affected in turn.

## Lighting conditions

Lighting conditions have an impact on how HoloLens perceives the environment and recognizes the space. Environments with unstable lighting conditions are prone to hologram instability. If the light changes significantly, HoloLens might consider the space as a new environment and build a new map for it. Previously visible features might be invisible and features that weren’t visible might be visible. 

## Feature patterns

HoloLens builds maps of its surroundings, and tracks its position and hologram position based on visible features (high contrast point and corners) in the environment. If the space in which HoloLens is operating has a low number of visible features (mostly white walls for example), or very repetitive patterns (textured surfaces), this will impact hologram position and stability as HoloLens won’t be able to properly identify and track uniquely specific points in the environment.

## Device wear (HoloLens 1 only)

HoloLens uses a novel display technology to project holograms in the operator's field of view. On HoloLens 1, the way that operators wear a device on their head has a huge impact on the perceived position of the holograms. The best way to understand this is to adjust the device positioning while aligning holograms to their physical counterparts in Dynamics 365 Guides. Notice how the alignment of holograms is affected when you shift the device left and right, up and down, or forward and backward. Operators should wear the device in a consistent way, and they should understand that subtle shifts in device positioning might not feel different but can cause significant changes in perceived hologram locations. On HoloLens 2, issues with device positioning are addressed through eye tracking.

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Anchoring overview|[Overview of anchoring a guide](pc-app-anchor.md)|
|Anchoring accuracy|[Learn about consistency of placement and expectations](pc-app-anchor-placement-consistency.md)|
|Creating types of anchors|[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|HoloLens app for authors|[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)|
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)
