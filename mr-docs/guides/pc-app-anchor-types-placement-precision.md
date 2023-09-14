---
author: davepinch
description: Learn about different anchor types and placement, and their effect on hologram precision in Dynamics 365 Guides. 
ms.author: davepinch
ms.date: 07/27/2021
ms.topic: conceptual
title: Anchor types and placement, and their effect on hologram precision in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Effect of anchor types/placement on hologram precision in Dynamics 365 Guides

Even if an author or operator perfectly places a holographic anchor or perfectly aligns the green outline when scanning a QR code or circular code anchor in Microsoft Dynamics 365 Guides, an anchor's position will never be perfectly precise and exactly the same as a previous placement or alignment. Very small (invisible) variations are introduced every time a user anchors a guide. This is particularly true for environments where the same guide is used on different devices and different users anchor the guide in very slightly different ways. 

Since a guide's holograms are placed relative to the anchor position and orientation, all hologram positions across the guide inherit a combination of position and orientation errors introduced when positioning or scanning anchors. These position and orientation errors are amplified if holograms are placed farther away from the anchor (known as the "lever-arm effect").

To maximize hologram position consistency so that the position of a hologram in the world stays the same across users and devices, whenever possible:

- Use QR or circular code anchors instead of holographic anchors for small to medium-sized objects and spaces. 

- Use [Object Anchors](pc-app-anchor-azure-object.md) for larger static objects. 

    The overall order of accuracy for the different kinds of anchors from most precise to least precise is:

    1. Object anchor

    1. QR code anchor

    1. Circular code anchor

    1. Holographic anchor

- Place holograms close to the anchor (not more than 3 meters away)

- Author from the operator's viewpoint

- Look at the hologram from the side to avoid depth position variation

- Scan anchors from the same position and angle

Each of these suggestions is covered in more detail in this article. 

> [!IMPORTANT]
> In addition to the suggestions included in this article, make sure to review the following articles:
>
> - [Effect of calibration, pre-scanning, and environment on positional precision of holograms](pc-app-anchor-improve-hologram-precision.md)
> - [Best practices for Object Anchors](pc-app-anchor-object-best-practices.md)
> - [Best practices for QR code anchors](pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors)
> - [Best practices for circular code anchors](pc-app-anchor-circular-code.md#best-practices-for-circular-code-anchors)
> - [Best practices for holographic anchors](pc-app-anchor-holographic.md#best-practices-for-holographic-anchors)

## Object Anchors

The Object Anchors feature uses a 3D model of an object to automatically detect and anchor to a real-world object. Use this anchor type as an alternative when you can't attach a physical marker to an object or near an object. With an object anchor, no printed marker is required; you just need a 3D capture of the object that HoloLens uses to recognize in the real world. Object anchors are recommended for larger static objects.   

[Learn more about Object Anchors](pc-app-anchor-azure-object.md).

## QR and circular code anchors

This anchor type relies on a printed physical marker that HoloLens recognizes by using different sets of sensors. 

During scanning, the position and orientation can suffer a small amount of angular error, which is usually not visible to the eye. This small angular error might not be perceptible when looking at the green outline used during the scanning process (which might seem perfectly aligned to the printed anchor) but will affect holograms that are positioned far away from the anchor. However, QR and circular code anchors provide much more accurate results than holographic anchors. QR code anchors are recommended for small and medium-sized objects and spaces when consistency of hologram position and alignment to real-world objects is crucial.

## Holographic anchors

Manually aligning holographic anchors with physical objects can be challenging, especially for holographic anchors that use larger holograms. Even when following best practices, different users will position holograms in slightly different ways whenever they anchor the guide. This small variation can have a big impact on hologram position across the guide. 

**For this reason, consider using holographic anchors when consistency of hologram position and alignment to real-world objects isn’t crucial (for example, for quick demos or virtual classroom training).**

## Placement of holograms in proximity to the anchor

Because it's very challenging to always maintain the exact same position and orientation, all anchor methods suffer from the "lever arm effect". Holograms that are close to the anchor will more likely be positioned consistently at the same location, while holograms that are farther away can suffer from important position variability between scans. **For this reason, one of the most important guidelines for authors is to place holograms close to their anchor for best positional consistency.** 

If alignment consistency with real-world objects is important, **don't place holograms more than 3 meters away from the anchor**. If your scenario needs to cover large spaces, you might want to split your steps into different guides to maximize position consistency. If that’s not possible, or if your scenario requires greater positional consistency than shown in the table above, contact the Dynamics 365 Guides team so we can better understand your scenario and address your feedback in future releases. 

## Author from the operator's viewpoint

A hologram's perceived position depends on the user’s view point. When an author places a hologram 1 meter in front of them, operators looking at this hologram from 3 meters might perceive it to be at a different location. As an author, to ensure consistency of hologram perceived position, make sure you are authoring from a viewpoint most likely to be used by your operators. 

## View holograms from the side to avoid depth position variation

When authoring, you're placing holograms in 3D space. Making sure the holograms are aligned with the expected target in terms of depth is crucial, as the smallest depth position variation can greatly impact the operator's perceived hologram position if viewed from a slightly different viewpoint. To ensure proper depth position, look at your hologram from the side and readjust if needed.  

## Scan anchors from the same position and angle

When re-anchoring a guide, whether you're an author or an operator, make sure to always scan the anchor from the same position and angle. Variation in the position and angle can result in inconsistencies in different HoloLens runs because the HoloLens sensors will have a very slightly different space perception. Even if the green outline in the QR code seems to be in the right place, micro errors can impact final accuracy, especially if holograms are placed far away from the anchor (lever arm effect).

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Anchoring overview|[Overview of anchoring a guide](pc-app-anchor.md)|
|Creating types of anchors|[Create an Object Anchor in the PC app](pc-app-anchor-azure-object.md)|
||[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|Hologram precision|[Effect of calibration, pre-scanning, and environment](pc-app-anchor-improve-hologram-precision.md)|
|HoloLens app for authors|[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)|
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
