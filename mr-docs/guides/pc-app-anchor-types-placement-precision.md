---
author: Mamaylya
description: Learn about different anchor types and placement, and their effect on hologram precision in Dynamics 365 Guides. 
ms.author: mamaylya
ms.date: 10/09/2020
ms.service: crm-online
ms.topic: article
title: Anchor types and placement, and their effect on hologram precision in Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Anchor types and placement, and their effect on hologram precision in Dynamics 365 Guides

Even if an author or operator perfectly places a holographic anchor or perfectly aligns the green outline when scanning a QR code or circular code anchor in Microsoft Dynamics 365 Guides, an anchor's position will never be perfectly precise and exactly the same as a previous placement or alignment. Very small (invisible) variations are introduced every time a user anchors a guide, especially in an environment where there are multiple users on multiple HoloLens devices. 

Since a guide's holograms are placed relative to the anchor position and orientation, all hologram positions across the guide inherit a combination of position and orientation errors introduced when positioning or scanning anchors. These position and orientation errors are amplified if holograms are placed farther away from the anchor (known as the "lever-arm effect").

To maximize hologram position consistency so that the position of a hologram in the world stays the same across users and devices, whenever possible:

- Use QR or circular code anchors instead of holographic anchors

- Place holograms close to the anchor (not more than 3 meters away)

- Author from the operator's viewpoint

- Look at the hologram from the side to avoid depth position variation

Each of these suggestions is covered in more detail in this article. 

> [!IMPORTANT]
> In addition to the suggestions included in this article, make sure to review the following articles:
>
> - [Improve positional precision of holograms](pc-app-anchor-improve-hologram-precision.md)
> - [Best practices for QR code anchors](pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors)
> - [Best practices for circular code anchors](pc-app-anchor-circular-code.md#best-practices-for-circular-code-anchors)
> - [Best practices for holographic anchors](pc-app-anchor-holographic.md#best-practices-for-holographic-anchors)

## QR and circular code anchors

This anchor type relies on a printed physical marker that HoloLens recognizes by using different sets of sensors. 

During scanning, the position and orientation can suffer a small amount of angular error, which is usually not visible to the eye. This small angular error might not be perceptible when looking at the green outline used during the scanning process (which might seem perfectly aligned to the printed anchor) but will affect holograms that are positioned far away from the anchor. However, QR and circular code anchors provide much more accurate results than holographic anchors. **QR code anchors are recommended when consistency of hologram position and alignment to real world objects is crucial.**

## Holographic anchors

Manually aligning holographic anchors with physical objects can be challenging, especially for holographic anchors that use larger holograms. Even when following best practices, different users will position holograms in slightly different ways whenever they anchor the guide. This small variation can have a big impact on hologram position across the guide. 

**For this reason, consider using holographic anchors when consistency of hologram position and alignment to real-world objects isn’t crucial (for example, for quick demos or virtual classroom training).**

## Placement of holograms in proximity to the anchor

Because it's very challenging to always maintain the exact same position and orientation, all anchor methods suffer from the "lever arm effect". Holograms that are close to the anchor will more likely be positioned consistently at the same location, while holograms that are farther away can suffer from important position variability between scans. **For this reason, one of the most important guidelines for authors is to place holograms close to their anchor for best positional consistency.** 

The following table shows what to expect on average for different anchor methods at different distances.

|Anchor method|Average hologram position variability when positioned <1m away from the anchor location (seen at arm's length)	|Average hologram position variability when <3m away from the anchor location (seen at arm's length)|
|-----------------------|--------------------------------------------------|--------------------------------------------------|
|QR code anchor|	5 to 10mm	|15 to 30mm|
|Circular code anchor|10 to 15mm|	30 to 45mm|
|Holographic anchor|	30mm	|90mm|

If alignment consistency with real-world objects is important, **don't place holograms more than 3 meters away from the anchor**. If your scenario needs to cover large spaces, you might want to split your steps into different guides to maximize position consistency. If that’s not possible, or if your scenario requires greater positional consistency than shown in the table above, contact the Dynamics 365 Guides team so we can better understand your scenario and address your feedback in future releases. 

## Author from the operator's viewpoint

A hologram's perceived position depends on the user’s view point. When an author places a hologram 1 meter in front of them, operators looking at this hologram from 3 meters might perceive it to be at a different location. As an author, to ensure consistency of hologram perceived position, make sure you are authoring from a viewpoint most likely to be used by your operators. 

## View holograms from the side to avoid depth position variation

When authoring, you're placing holograms in 3D space. Making sure the holograms are aligned with the expected target in terms of depth is crucial, as the smallest depth position variation can greatly impact the operator's perceived hologram position if viewed from a slightly different viewpoint. To ensure proper depth position, look at your hologram from the side and readjust if needed.  

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Anchoring overview|[Overview of anchoring a guide](pc-app-anchor.md)|
|Creating types of anchors|[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|Hologram precision|[Improve positional precision of holograms](pc-app-anchor-improve-hologram-precision.md)|
|HoloLens app for authors|[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)|
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)
