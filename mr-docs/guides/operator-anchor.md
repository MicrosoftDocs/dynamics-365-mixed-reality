---
author: Mamaylya
description: Learn how to anchor a guide in the Microsoft Dynamics 365 Guides HoloLens app if you're an operator.
ms.author: mamaylya
ms.date: 07/30/2021
ms.topic: article
title: Anchor a guide in the Dynamics 365 Guides HoloLens app (operators)
ms.reviewer: v-bholmes
---

# Anchor a guide in the Dynamics 365 Guides HoloLens app (for operators)

When you open a guide in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], the first thing that you see is the anchoring instructions for the guide. For example, if a QR code is used to anchor the guide, you see the **Scan QR code** page.

![Scan QR code page.](media/qr-code-scan.jpg "Scan QR code page")

Like the calibration of [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)], anchoring a guide is a crucial step. You anchor a guide to make sure that the holographic instructions line up with your real-world environment. If the holograms don't line up, you'll likely be confused when you try to do a task. You could even cause damage. For example, you might drill a hole in the wrong place.

## Four types of anchors

The way that you anchor your guide depends on the type of anchor that the author selected for the guide. There are four types of anchors: 

- Object anchor

- QR code anchor

- Circular code anchor

- Holographic anchor

This topic provides step-by-step instructions for each type of anchor.

## Anchor a guide by using an object anchor (Azure Object Anchors Preview)

1. Put on your HoloLens, and then locate the target object in your physical environment.

2. In the **Scan target object** dialog box, select **Initiate Scan**.

     ![Scan Target Object dialog box.](media/azure-object-scan.jpg "Scan Target Object dialog box")
 
3. Look at the target object with your HoloLens, and then move around the object to scan it. 

    HoloLens automatically recognizes the object based on the object anchor. 

4. Continue to move around the object if you're prompted to do so.

    ![Move around the target object screen.](media/AOA-move-around.PNG "Move around the target object screen") 
  
5. When the scan is successful, the object will have a green overlay.

    > [!NOTE]
    > Objects that have moved or are moving may cause variable accuracy. If you have issues with object detection and content alignment, try clearing the mesh and all holograms. To do this, on HoloLens, go to **Settings** > **System** > **Holograms** > **Remove all holograms**. This will clear the location of all holograms placed in your world, not just the object anchor.

6. If this is your first time scanning the object, select **Confirm** or **Rescan**. If the object has been scanned previously, the guide will be successfully anchored to the object anchor. HoloLens automatically goes to the first step of the guide. 
 
## Anchor your guide by using a QR code anchor

1. Look for a QR code anchor that's attached to a physical object in your real-world environment. The QR code anchor will resemble this illustration.

    ![QR code anchor.](media/qr-code-example.PNG "QR code anchor")

2. Put on your HoloLens and open the guide. If a QR code is used to anchor the guide, you'll see the **Scan QR code** page.

3. On the **Scan QR code** page, select **Initiate Scan**. 

    ![Initiate Scan button on the Scan QR code page.](media/qr-code-scan.jpg "Initiate Scan button on the Scan QR code page")

4. On your [!include[pn-hololens](../includes/pn-hololens.md)], you'll see a hologram that resembles the QR code anchor. Align the anchor hologram with the QR code anchor. When the green box is aligned, gaze at **Confirm** to select it.
    
    ![Confirm button on the QR Code Anchor Found page.](media/qr-code-confirm.jpg "Confirm button on the QR Code Anchor Found page")
    
    > [!TIP]
    > You can re-align holographic content that might seem offset from the real world (for example, a rectangle that should be referencing a tool, but is floating in the air away from the tool bench). When using a QR code anchor, a good way to control hologram offset is to make sure the green outline aligns with the QR code. If the green outline isn’t aligned, you may need to tap the **Anchor** button to rescan. 

## Anchor your guide by using a circular code anchor

1. Look for a circular code anchor that's attached to a physical object in your real-world environment. The circular code anchor will resemble this illustration.

    ![Circular code anchor.](media/circular-code-example.PNG "Circular code anchor")

2. Put on your HoloLens and open the guide. If a circular code is used to anchor the guide, you'll see the **Scan circular code** page.

3. On the **Scan circular code** page, select **Initiate Scan**. 

    ![Initiate Scan button on the Scan Circular code page.](media/circular-code-scan.jpg "Initiate Scan button on the Scan Circular code page")

4. On your [!include[pn-hololens](../includes/pn-hololens.md)], you'll see a hologram that resembles the circular code anchor. Align the anchor hologram with the circular code anchor. When the green box is aligned, gaze at **Confirm** to select it.

    ![Confirm button on the Circular Code page.](media/circular-code-confirm.jpg "Confirm button on the Circular Code page")
    
    > [!TIP]
    > You can re-align holographic content that might seem offset from the real world (for example, a rectangle that should be referencing a tool, but is floating in the air away from the tool bench). When using a circular code anchor, a good way to control hologram offset is to make sure the green outline aligns with the circular code. If the green outline isn’t aligned, you may need to tap the **Anchor** button to rescan. 

## Anchor your guide by using a holographic anchor

For a holographic anchor, you align a hologram on your [!include[pn-hololens](../includes/pn-hololens.md)] with a similar object in the real world. 

To align the holographic anchor with its real-world counterpart, air tap and hold to move the hologram. Tap and hold the blue spheres to rotate the hologram as required.

![Rotating a holographic anchor.](media/rotate-holographic-anchor.jpg "Rotating a holographic anchor")

> [!TIP]
> You can re-align holographic content that might seem offset from the real world (for example, a rectangle that should be referencing a tool, but is floating in the air away from the tool bench). When using a holographic anchor, select the **Anchor** button to make sure the digital version of the real object and the object itself are still aligned.

## Where alignment information is stored

When you align your guide, if you're using the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] Commercial Suite, the alignment information is stored on [!include[pn-hololens](../includes/pn-hololens.md)], so you don't have to realign the guide every time that you open it. However, you can realign a guide at any time if you think that the holograms are out of alignment by using the **Anchor** button. For more information, see [Operate a guide](operator-step-card-orientation.md).

## What's next?

- [Calibrate your HoloLens](operator-calibrate-hl2)
- [Install the app and sign in](hololens-app-install-sign-in.md)
- [Gestures for navigating the app](operator-gestures.md)
- [Operate a guide](operator-step-card-orientation.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
