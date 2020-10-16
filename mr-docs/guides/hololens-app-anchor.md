---
author: Mamaylya
description: Learn how to anchor a guide when you're using the Microsoft Dynamics 365 Guides HoloLens app in Author mode.
ms.author: mamaylya
ms.date: 10/01/2020
ms.service: crm-online
ms.topic: article
title: Anchor a guide in Author mode by using the Dynamics 365 Guides HoloLens app 
ms.reviewer: v-brycho
---

# Anchor a guide in the Dynamics 365 Guides HoloLens app (for authors)

When you open a guide in the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] HoloLens app, the first thing that you see is the anchoring instructions that were created in the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC app. The method that you use to anchor the guide depends on the type of anchor that was created in the PC app. For more information about how to create an anchor, and the types of anchors, see [Anchor your guide to the real world in Dynamics 365 Guides PC app](anchor.md).

## Anchor a guide by using a QR code anchor

1. Put on your HoloLens, and stand about two feet in front of the QR code anchor.

2. On the **Scan QR Code Anchor** page, select **Initiate Scan**.

    ![Initiate Scan button on the Scan QR Code Anchor page](media/qr-code-scan.PNG "Initiate Scan button on the Scan QR Code Anchor page")

3. With your [!include[pn-hololens](../includes/pn-hololens.md)], look at the QR code anchor until a green outline appears. Use your gaze to align the green box with the anchor, and then select **Confirm**.

    ![Aligning with the QR code anchor](media/qr-code-green-outline.PNG "Aligning with the QR code anchor")

4. On the **QR Code Anchor Found** page, select **Confirm**.

    ![Confirm button on the QR Code Anchor Found page](media/qr-code-confirm.PNG "Confirm button on the QR Code Anchor Found page")
    
    >[!TIP]
    >You can re-align holographic content that might seem offset from the real world (for example, a rectangle that should be highlighting a tool, but is floating in the air away from the tool bench). When using a QR code anchor, a good way to control hologram offset is to make sure the green outline aligns with the QR code. If the green outline isn’t aligned, you may need to tap the **Anchor** button to rescan. 

## Anchor a guide by using a circular code anchor

1. Put on your HoloLens, and stand about two feet in front of the circular code anchor.

2. On the **Scan Circular Code Anchor** page, select **Initiate Scan**.

    ![Initiate Scan button on the Scan Circular Code Anchor page](media/circular-code-scan.PNG "Initiate Scan button on the Scan Circular Code Anchor page")

    On your [!include[pn-hololens](../includes/pn-hololens.md)], you will see a holographic image that looks like the following illustration.

    ![Holographic image of circular code](media/circular-code-hologram.PNG "Holographic image of circular code")

3. With your [!include[pn-hololens](../includes/pn-hololens.md)], look at the circular code anchor until a green outline appears. Use your gaze to align the green box with the anchor, and then select **Confirm**.

    ![Aligning with the circular code anchor](media/circular-code-green-outline.PNG "Aligning with the circular code anchor")

4. On the **Circular Code Anchor Found** page, select **Confirm**.

    ![Confirm button on the Circular Code Anchor Found page](media/circular-code-confirm.PNG "Confirm button on the Circular Code Anchor Found page")
    
    >[!TIP]
    >You can re-align holographic content that might seem offset from the real world (for example, a rectangle that should be highlighting a tool, but is floating in the air away from the tool bench). When using a circular code anchor, a good way to control hologram offset is to make sure the green outline aligns with the circular code. If the green outline isn’t aligned, you may need to tap the **Anchor** button to rescan. 

## Anchor a guide by using a holographic anchor

- Use air tap and hold to move the holographic anchor and align it to its real-world counterpart. To rotate the anchor, tap and hold the blue spheres. On [!include[pn-hololens](../includes/pn-hololens.md)] 2, you can use your hand to directly select and place a digital anchor when you author a guide.

    ![Rotating a holographic anchor](media/rotate-digital-anchor.PNG "Rotating a holographic anchor")

    >[!TIP]
    >You can re-align holographic content that might seem offset from the real world (for example, a rectangle that should be highlighting a tool, but is floating in the air away from the tool bench). When using a holographic anchor, select the **Anchor** button to make sure the digital version of the real object and the object itself are still aligned. 

## Re-anchor a guide

When you anchor your guide, the anchoring information is stored on your [!include[pn-hololens](../includes/pn-hololens.md)]. Therefore, you don't have to re-anchor the guide every time that you open it. However, you can use the **Anchor** button to re-anchor a guide at any time, if you feel that the holograms are out of alignment. For more information, see [Place holograms, add styles, and more](hololens-app-orientation.md)

> [!NOTE]
> To help guarantee accurate placement of 3D content, you might have to adjust the hardware offset on [!include[pn-hololens](../includes/pn-hololens.md)] 1 devices. For more information, see [How do I address hardware offset in HoloLens 1 devices to ensure accurate placement of holograms for printed anchor alignment](https://docs.microsoft.com/dynamics365/mixed-reality/guides/known-issues#how-do-i-address-hardware-offset-in-hololens-1-devices-to-ensure-accurate-placement-of-holograms-for-circular-code-anchor-alignment).

## What's next?

Use the following table to find more information on anchoring.

|Area|Link|
|----------------------|------------------------------------------------------------------|
|Anchoring overview|[Overview of anchoring a guide](pc-app-anchor.md)|
|Creating types of anchors|[Create a QR code anchor in the PC app](pc-app-anchor-qr-code.md)|
||[Create a circular code anchor in the PC app](pc-app-anchor-circular-code.md)|
||[Create a holographic anchor in the PC app](pc-app-anchor-holographic.md)|
||[Change from one anchoring type to another in the PC app](pc-app-anchor-change-type.md)|
|Hologram precision|[Effect of calibration, pre-scanning, and environment](pc-app-anchor-improve-hologram-precision.md)|
||[Effect of anchor types/placement](pc-app-anchor-types-placement-precision.md)
|HoloLens app for operators|[Anchor your guide as an operator in the HoloLens app](operator-anchor.md)
