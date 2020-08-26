---
author: Mamaylya
description: Get an overview anchoring holograms in Microsoft Dynamics 365 Guides, using a QR code anchor, circular code anchor, or holographic anchor.
ms.author: mamaylya
ms.date: 03/24/2020
ms.service: crm-online
ms.topic: article
title: Overview of anchoring your guide to the real world in the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Overview of anchoring your guide to the real world in the Dynamics 365 Guides PC app

When you create a guide by using the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC app, one of the 
first steps is to select an anchoring method. When you anchor a guide, you spatially synchronize it with your real-world environment (for example, a factory floor). Anchors 
help holograms determine where they are in the real world. You must create an anchor for your guide before it will work on [!include[pn-hololens](../includes/pn-hololens.md)].

![Worker attaching a QR code anchor to machine](media/anchor-overview.PNG "Worker attaching a QR code anchor to machine")

It's crucial to ensure that holograms are aligned as precisely as possible. If holograms are misaligned, your instructions may show actions at incorrect locations, 
which can result in operator confusion or damage to parts.

## Three ways to anchor a guide

There are three ways to anchor a guide:

- **QR code anchor (recommended)**. When you use a QR code anchor, you align your guide by gazing at a printed QR code anchor that's attached to a physical object in the real world. QR code anchoring is recommended, because it's the most accurate method, and you can print the anchor at different sizes. 

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

- [Create a QR code anchor](pc-app-anchor-qr-code.md)

- [Create a circular code anchor](pc-app-anchor-circular-code.md)

- [Create a holographic anchor](pc-app-anchor-holographic.md)

After creating the anchor in the PC app, you use the HoloLens app to anchor your guide in the real world, whether you're an author or operator. Use the following links to learn how to anchor a guide, depending on whether you're an author or an operator:

- [Anchor a guide if you're an author](hololens-app-anchor.md)

- [Anchor a guide if you're an operator](operator-anchor.md)

## What's next?

## What's next?

[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)<br>
[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)<br>
[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)<br>
[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)<br>
[Anchor your guide as an author in the HoloLens app](hololens-app-anchor.md)<br>
[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)<br>
