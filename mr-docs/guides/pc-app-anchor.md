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
first steps is to select an anchoring method. When you anchor a guide, you spatially synchronize with to your real-world environment (for example, a factory floor). Anchors 
help holograms determine where they are in the real world. You must create an anchor for your guide before it will work on [!include[pn-hololens](../includes/pn-hololens.md)].

![Worker attaching a QR code anchor to machine](media/anchor-overview.PNG "Worker attaching a QR code anchor to machine")

It's crucial to ensure that your guide alignment is correct and as precise as possible. If the guide is misaligned, your instructions may show actions at incorrect locations, 
which can result in operator confusion or damage to parts.

## Three ways to anchor a guide

There are three ways to anchor a guide:

- **QR code anchor (recommended)**. When you use a QR code anchor, you align a guide by gazing at (scanning) a printed QR code anchor that is attached to a physical object in the real world. QR code anchoring is recommended, because it's the most accurate method, and you can print the anchor at different sizes. QR code anchors are new in the February 2020 release of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

    > [!NOTE]
    > QR code anchoring isn't available on HoloLens 1 devices.

- **Circular code anchor**. When you use a circular code anchor, you align a guide by gazing at (scanning) a printed circular code anchor that is attached to a physical object in the real world. (Circular code anchors are referred to as printed anchors in earlier versions of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].)

- **Holographic anchor**. When you use a holographic anchor, you align a guide to a digital 3D hologram that is overlaid on a physical object in the real world. (Holographic anchors are referred to as digital anchors in earlier versions of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].) Here are some reasons why you might have to use a holographic anchor:

    - It isn't feasible to attach a QR code anchor or circular code anchor, because the location where the guide is authored differs from the location where the parts are.

    - It isn't feasible to attach a QR code anchor or circular code anchor because of moving parts.

    - You can't guarantee that the placement of the QR code anchor or circular code anchor will be the same every time.

    - A part is too small to attach a QR code anchor or circular code anchor to it.

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] includes an **Anchor** wizard that makes it easy to select and set up the most appropriate anchor type for your situation.

## What's next?

[Structure your guide in the Outline page](structure-guide.md)<br>
[Create steps and add 3D content or 2D media](create-steps-assign-media.md)<br>
[Add a website or Power Apps link to a step](pc-app-website-powerapps-link.md)<br>
[Create and copy a link to a guide or step](pc-app-copy-link-guide-step.md)<br>
[Learn about keyboard shortcuts](keyboard-shortcuts-pc-app.md)<br>
[Deactivate a guide](pc-app-deactivate-guide.md)<br>
[Add a website or Power Apps link to a step](pc-app-website-powerapps-link.md)<br>
[Learn about keyboard shortcuts](keyboard-shortcuts-pc-app.md)<br>
[Learn what makes a great mixed reality guide](great-guide.md)
