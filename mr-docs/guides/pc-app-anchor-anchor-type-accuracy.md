---
author: Mamaylya
description: Learn about the importance of placement consistency when anchoring a guide with the Dynamics 365 Guides PC app
ms.author: mamaylya
ms.date: 10/09/2020
ms.service: crm-online
ms.topic: article
title: Consistency of placement and expectations when anchoring a guide in the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Anchor types: positional accuracy of holograms in Dynamics 365 Guides

Since holograms are located relative to a virtual reference frame placed when an author or operator is positioning a holographic anchor or scanning a QR/circular code anchor in Microsoft Dynamics 365 Guides, they can inherit position errors and amplify orientation errors introduced when positioning or scanning. The consistency of the virtual reference frame placement is key to keeping holograms consistently aligned to the same real-world objects across multiple alignments by different users on different devices. Any inconsistency greatly impacts the position of the holograms.

A small position error will cause a consistent offset for all the holograms in a guide. A small orientation error is even worse; the hologram offset increases as the user moves away from the anchor (“lever-arm effect”). 

To maximize hologram position consistency so that the position of a hologram in the world stays the same across users and devices, it’s very important to ensure that the virtual reference frame is consistently positioned and oriented exactly the same way. 

Microsoft research also shows that different anchoring methods provide different results across users and devices. 

> [!IMPORTANT]
> In addition to the suggestions included in this article, make sure to review best practices for each type of anchor:
>
> - [Best practices for QR code anchors](pc-app-anchor-qr-code.md#best-practices-for-qr-code-anchors)
> - [Best practices for circular code anchors](pc-app-anchor-circular-code.md#best-practices-for-circular-code-anchors)
> - [Best practices for holographic anchors](pc-app-anchor-holographic.md#best-practices-for-holographic-anchors)
>
> Also, make sure that you consistently place or scan the anchor the same way each time.

## Holographic anchors

Manually aligning holographic anchors with physical objects can be challenging especially for holographic anchors that use larger holograms. Even when following best practices, different users will position holograms in slightly different ways whenever they anchor the guide. This small variation can have a big impact on hologram position across the guide. 

**For this reason, consider using holographic anchors when consistency of hologram position and alignment to real-world objects isn’t crucial (for example, for quick demos or virtual classroom training).**

## QR and circular code anchors

This anchor type relies on a printed physical marker that HoloLens recognizes by using different sets of sensors. 

During scanning, the position of the virtual reference frame and its orientation can suffer a small amount of angular error, which is usually not visible to the eye. This small angular error might not be perceptible when looking at the green outline used during the scanning process (which might seem perfectly aligned to the printed anchor) but will affect holograms that are positioned far away from the anchor. However, QR and circular code anchors provide much more accurate results than holographic anchors. **QR code anchors are recommended when consistency of hologram position and alignment to real world objects is crucial.**

## Summary of positional consistency per anchor method

Because it's very challenging to always position the virtual reference frame the same way during the anchoring process, all anchor methods suffer from the "lever arm effect". Holograms that are close to the anchor will more likely be positioned consistently at the same location, while holograms that are farther away can suffer from important position variability between scans. **For this reason, one of the most important guidelines for authors is to place holograms close to their anchor for best positional consistency.** 

The following summary table shows what can be expected on average.

|Anchor method|Average hologram position variability when positioned <1m away from the anchor location (and seen at arm's length)	|Average hologram position variability when <3m away from the anchor location (when seen at arm's length)|
|-----------------------|--------------------------------------------------|--------------------------------------------------|
|QR code anchor|	5 to 10mm	|15 to 30mm|
|Circular code anchor|10 to 15mm|	30 to 45mm|
|Holographic anchor|	30mm	|90mm|

- If alignment consistency with real-world objects is important, don't place holograms more than 3 meters away from the anchor. If your scenario needs to cover large spaces, you might want to split your steps into different guides to maximize position consistency. If that’s not possible, or if your scenario requires greater positional consistency than shown in the table above, contact the Dynamics 365 Guides team so we can better understand your scenario and address your feedback in future releases. 

- A hologram's perceived position depends on the user’s view point. When an author places a hologram 1 meter in front of them, operators looking at this hologram from 3 meters might perceive it to be at a different location. As an author, to ensure consistency of hologram perceived position, make sure you are authoring the position from a viewpoint most likely to be used by your operators. 

- When authoring, you're placing holograms in 3D space. Making sure the holograms are aligned with the expected target in terms of depth is crucial, as the smallest depth position variation can greatly impact the operator's perceived hologam position if viewed from a slightly different viewpoint. To ensure proper depth position, look at your hologram from the side and readjust if needed.  

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Anchoring overview|[Overview of anchoring a guide](pc-app-anchor.md)|
|Anchoring accuracy|[Things that affect positional consistency](pc-app-anchor-parameters-positional-consistency.md)|
|Creating types of anchors|[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|HoloLens app for authors|[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)|
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)
