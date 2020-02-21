---
author: Mamaylya
description: Learn how to anchor a guide in the Microsoft Dynamics 365 Guides HoloLens app if you're an operator.
ms.author: mamaylya
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Anchor a guide in the Dynamics 365 Guides HoloLens app as an operator
ms.reviewer: v-brycho
---

# Anchor a guide in the Dynamics 365 Guides HoloLens app (for operators)

The first thing you see when you open a guide in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] is the anchoring instructions for the guide. For example, if the guide is anchored with a QR code, you'll see the following screen.

![Scan QR Code Anchor page](media/qr-code-scan.PNG "Scan QR Code Anchor page")

Like the calibration of [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)], anchoring a guide is a crucial step. You anchor a guide to make sure that the holographic instructions line up with your real-world environment. If the holograms don't line up, you'll likely be confused when you try to do a task. You could even cause damage. For example, you might drill a hole in the wrong place.

## Three types of anchors

How you anchor your guide depends on the type of anchor the author chose for the guide. There are three types of anchors: 

- QR code anchor

- Circular code anchor

- Holographic anchor

This article provides step-by-step instructions for each type of anchor.

## Anchor your guide by using a QR code anchor

1. Look for a QR code anchor that's attached to a physical object in your real-world environment. The QR code anchor will resemble this illustration.

    ![QR code anchor](media/qr-code-example.PNG "QR code anchor")
    
2. Put on your HoloLens and open the guide. If the guide is anchored with a QR code, you'll see the **Scan QR Code Anchor** page.

3. In the **Scan QR Code Anchor** page, select **Initiate Scan**. 

    ![QR code scan](media/qr-code-scan.PNG "QR code scan")

3. On your [!include[pn-hololens](../includes/pn-hololens.md)], you'll see a hologram that resembles the QR code anchor. Align the anchor hologram with the QR code anchor. When the green box is aligned, gaze at **Confirm** to select it.

    ![QR code alignment](media/qr-code-green-outline.PNG "QR code alignment")

4. In the **QR Code Anchor Found** page, select **Confirm**.

    ![QR Code Anchor Found page](media/qr-code-confirm.PNG "QR Code Anchor Found page")


## Anchor your guide by using a circular code anchor

1. Look for a circular code anchor that's attached to a physical object in your real-world environment. The circular code anchor will resemble this illustration.

    ![Circular code anchor](media/circular-code-example.PNG "Circular code anchor")
    
2. Put on your HoloLens and open the guide. If the guide is anchored with a circular code, you'll see the **Scan Circular Code Anchor** page.

3. In the **Scan Circular Code Anchor** page, select **Initiate Scan**. 

    ![QR code scan](media/circular-code-scan.PNG "QR code scan")

4. On your [!include[pn-hololens](../includes/pn-hololens.md)], you'll see a hologram that resembles the circular code anchor. Align the anchor hologram with the circular code anchor. When the green box is aligned, gaze at **Confirm** to select it.

    ![Holographic marker](media/circular-code-green-outline.PNG "Holographic marker")

5. In the **Circular Code Anchor Found** page, select **Confirm**.

    ![Circular Code Anchor Found page](media/circular-code-confirm.PNG "Circular Code Anchor Found page")

## Anchor your guide by using a holographic anchor

For a holographic anchor, you align a hologram on your [!include[pn-hololens](../includes/pn-hololens.md)] with a similar object in the real world. For example, the following illustration shows a holographic anchor being aligned with its physical counterpart in the real world.

![Holographic anchor example](media/digital-anchor-example.PNG "Holographic anchor example")

To align the holographic anchor with its real-world counterpart, air tap and hold to move the hologram. Tap and hold the blue spheres to rotate the hologram as required.

![Rotating a holographic anchor](media/rotate-digital-anchor.PNG "Rotating a holographic anchor")

## Where alignment information is stored

When you align your guide, if you're using the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] Commercial Suite, the alignment information is stored on [!include[pn-hololens](../includes/pn-hololens.md)], so you don't have to realign the guide every time that you open it. However, you can realign a guide at any time if you think that the holograms are out of alignment by using the **Anchor** button. For more information, see [Operate a guide](operator-orientation.md).

## What's next?

[Calibrate your HoloLens](operator-calibrate.md)<br>
[Install the app and sign in](install-sign-in-operator.md)<br>
[Gestures for navigating the app](operator-gestures.md)<br>
[Operate a guide](operator-orientation.md)
