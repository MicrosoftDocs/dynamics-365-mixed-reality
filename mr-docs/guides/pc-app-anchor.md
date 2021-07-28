---
author: Mamaylya
description: Get an overview anchoring holograms in Microsoft Dynamics 365 Guides, using a QR code anchor, circular code anchor, or holographic anchor.
ms.author: mamaylya
ms.date: 07/26/2021
ms.topic: article
title: Overview of anchoring your guide to the real world in the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
ms.custom: "intro-internal"
---

# Overview of anchoring your guide to the real world in the Dynamics 365 Guides PC app

When you create a guide by using the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC app, one of the 
first steps is to select an anchoring method. When you anchor a guide, you spatially synchronize it with your real-world environment (for example, a factory floor). Anchors 
help holograms determine where they are in the real world. You must create an anchor for your guide before it will work on [!include[pn-hololens](../includes/pn-hololens.md)].

![Worker attaching a QR code anchor to machine.](media/anchor-overview.PNG "Worker attaching a QR code anchor to machine")

It's crucial to ensure that holograms are aligned as precisely as possible. If holograms are misaligned, your instructions may show actions at incorrect locations, 
which can result in operator confusion or damage to parts.

## How does anchoring work?

Dynamics 365 Guides uses a single anchor per guide. It can be a digital (holographic) anchor or a physical anchor (QR code or circular code) that you print. 

When an operator places the holographic anchor or scans the physical anchor, Dynamics 365 Guides creates a virtual in-world reference frame at that location. All the holograms included in the guide are located in space relative to that virtual reference frame. 

If the holographic anchor is repositioned or the QR/circular code is rescanned, the reference frame is reset to match the updated digital or physical position of the anchor. 
Because HoloLens knows and remembers the space around the operator, it can remember the reference frame of a guide so operators don’t need to place the holographic anchor again or scan again. 

## Four ways to anchor a guide

There are four ways to anchor a guide:

- **Azure Object Anchors Preview** (recommended for larger static objects). Azure Object Anchors uses sensing and processing on HoloLens 2 to detect a digital model and align it to a physical object. You use the Guides model-driven app to convert an online 3D model to an object anchor, and then assign it to a guide. 

    Azure Object Anchors offers the following advantages over other types of anchors:

   - You don’t have to attach a physical marker to an object; the object is the anchor  

   - Avoids potential human error when placing markers or with wear and tear of a marker over time 

   - You can convert an existing 3D object model into an object anchor 

   - Improved alignment accuracy and reliability  

- **QR code anchor (recommended for small to medium size objects and spaces)**. When you use a QR code anchor, you align your guide by gazing at a printed QR code anchor that's attached to a physical object in the real world. QR code anchoring is recommended for small to medium size objects and spaces because it's the most accurate method, and you can print the anchor at different sizes. 

    > [!NOTE]
    > QR code anchoring isn't available on HoloLens 1 devices.

- **Circular code anchor**. When you use a circular code anchor, you align your guide by gazing at a printed circular code anchor that's attached to a physical object in the real world. 

- **Holographic anchor**. When you use a holographic anchor, you align your guide to a digital 3D hologram that's overlaid on a physical object in the real world. You might have to use a holographic anchor if:

    - It isn't feasible to attach a QR code anchor or circular code anchor because the guide is authored in a different location than where the parts are.

    - It isn't feasible to attach a QR code anchor or circular code anchor because of moving parts.

    - You can't guarantee that the placement of the QR code anchor or circular code anchor will be the same every time.

    - A part is too small to attach a QR code anchor or circular code anchor.

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] includes an **Anchor** wizard that makes it easy to select and set up the most appropriate anchor type for your situation.

## Overall process for creating anchors

Ragardless of which type of anchor you want to create, you always start with the Anchor wizard in the PC app. Use the following links to learn how to create different types of anchors in the PC app.

- [Create an Azure Object Anchor](pc-app-anchor-azure-object.md)

- [Create a QR code anchor](pc-app-anchor-qr-code.md)

- [Create a circular code anchor](pc-app-anchor-circular-code.md)

- [Create a holographic anchor](pc-app-anchor-holographic.md)

After creating the anchor in the PC app, you use the HoloLens app to anchor your guide in the real world, whether you're an author or operator. Use the following links to learn how to anchor a guide, depending on whether you're an author or an operator:

- [Anchor a guide if you're an author](hololens-app-anchor.md)

- [Anchor a guide if you're an operator](operator-anchor.md)

## Positional precision of holograms 

For information on the positional precision of holograms, make sure to see these articles:

- [Effect of calibration, pre-scanning, and environment](pc-app-anchor-improve-hologram-precision.md)
- [Effect of anchor types and placement](pc-app-anchor-types-placement-precision.md)

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Creating an anchor|[Create an Azure Object Anchor](pc-app-anchor-azure-object.md)|
||[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|Hologram precision|[Effect of calibration, pre-scanning, and environment](pc-app-anchor-improve-hologram-precision.md)|
||[Effect of anchor types/placement](pc-app-anchor-types-placement-precision.md)
|HoloLens app for authors|[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)|
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
