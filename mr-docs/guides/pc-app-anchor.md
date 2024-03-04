---
author: davepinch
description: Get an overview anchoring holograms in Microsoft Dynamics 365 Guides, using a QR code anchor, circular code anchor, or holographic anchor.
ms.author: davepinch
ms.date: 09/19/2023
ms.topic: overview
title: Overview of anchoring your guide to the real world in the Dynamics 365 Guides PC app
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Overview of anchoring your guide to the real world in the Dynamics 365 Guides PC app

When you create a guide by using the Microsoft Dynamics 365 Guides PC app, one of the first steps is to select an anchoring method. When you anchor a guide, you spatially synchronize it with your real-world environment (for example, a factory floor). Anchors help holograms determine where they are in the real world. You must create an anchor for your guide before it works on HoloLens.

![Worker attaching a QR code anchor to machine.](media/anchor-overview.PNG "Worker attaching a QR code anchor to machine")

It's crucial to ensure that holograms are aligned as precisely as possible. If holograms are misaligned, your instructions may show actions at incorrect locations, which can result in operator confusion or damage to parts.

## How does anchoring work?

Dynamics 365 Guides uses a single anchor per guide. It can be a digital anchor or a physical anchor that you print. 

When an operator places the holographic anchor or scans the physical anchor, Dynamics 365 Guides creates a virtual in-world reference frame at that location. All the holograms included in the guide are located in space relative to that virtual reference frame. 

If the digital anchor is repositioned or the printed anchor is rescanned, the reference frame is reset to match the updated digital or physical position of the anchor. Because HoloLens knows the space around the operator, it can remember the reference frame of a guide so operators don’t need to place the holographic anchor again or scan again. 

## Four ways to anchor a guide

There are four ways to anchor a guide:

- **Object anchors** (recommended for larger static objects). Object anchors uses sensing and processing on HoloLens 2 to detect a digital model and align it to a physical object. You use the Guides model-driven app to convert an online 3D object to an object anchor, and then assign it to a guide. 

  Object anchors offers the following advantages over other types of anchors:

  - You don’t have to attach a physical marker to an object; the object is the anchor.  

  - Avoids potential human error when placing markers or with wear and tear of a marker over time.

  - You can convert an existing 3D object model into an object anchor.

  - Improved alignment accuracy and reliability. 

- **QR code anchor (recommended for small to medium-size objects and spaces)**. When you use a QR code anchor, you align your guide by gazing at a printed QR code anchor that's attached to a physical object in the real world. QR code anchoring is recommended for small to medium-size objects and spaces because it's the most accurate method, and you can print the anchor at different sizes. 

  > [!NOTE]
  > QR code anchoring isn't available on HoloLens 1 devices.

- **Circular code anchor**. When you use a circular code anchor, you align your guide by gazing at a printed circular code anchor that's attached to a physical object in the real world. 

- **Holographic anchor**. When you use a holographic anchor, you align your guide to a digital representation that's overlaid on a physical object in the real world. The digital representation can be a computer-aided design (CAD) model or a scanned model.

  You might have to use a holographic anchor if:

  - It isn't feasible to attach a QR code anchor or circular code anchor because the guide is authored in a different location than where the parts are.

  - It isn't feasible to attach a QR code anchor or circular code anchor because of moving parts.

  - You can't guarantee that the placement of the QR code anchor or circular code anchor will be the same every time.

  - A part is too small to attach a QR code anchor or circular code anchor.

   > [!NOTE]
   > An [object anchor](pc-app-anchor-object.md) is preferred over a holographic anchor when:
   > - The target object is [suitable for object detection](pc-app-anchor-object-best-practices.md)
   > - Accuracy needs are high
   > - The target object is available in the real world to scan with HoloLens
   > - Holograms need to be consistently positioned at the same location

Dynamics 365 Guides includes an **Anchor** wizard that makes it easy to select and set up the most appropriate anchor type for your situation.

## Overall process for creating anchors

Regardless of which type of anchor you want to create, you always start with the Anchor wizard in the PC app. Use the following links to learn how to create different types of anchors in the PC app.

- [Create an object anchor](pc-app-anchor-object.md)

- [Create a QR code anchor](pc-app-anchor-qr-code.md)

- [Create a circular code anchor](pc-app-anchor-circular-code.md)

- [Create a holographic anchor](pc-app-anchor-holographic.md)

After creating the anchor in the PC app, you use the HoloLens app to anchor your guide in the real world, whether you're an author or operator. Use the following links to learn how to anchor a guide, depending on whether you're an author or an operator:

- [Anchor a guide if you're an author](hololens-app-anchor.md)

- [Anchor a guide if you're an operator](operator-anchor.md)

## Positional precision of holograms 

For information on the positional precision of holograms, review these articles:

- [Effect of calibration, prescanning, and environment](pc-app-anchor-improve-hologram-precision.md)
- [Effect of anchor types and placement](pc-app-anchor-types-placement-precision.md)

## Next steps

- [Create an object anchor in the PC app](pc-app-anchor-object.md)
- [Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)
- [Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)
- [Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)
- [Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
