---
author: Mamaylya
description: Learn how to anchor holograms in the Microsoft Dynamics 365 Guides PC app by using a QR code anchor
ms.author: mamaylya
ms.date: 10/01/2020
ms.service: crm-online
ms.topic: article
title: Anchor a guide in the Dynamics 365 Guides PC app by using a QR code anchor
ms.reviewer: v-brycho
---

# Anchor a guide in the Dynamics 365 Guides PC app by using a QR code anchor

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about creating a QR code anchor](https://youtu.be/NhdBG3emNUs)

You can anchor your guide to the real world in Microsoft Dynamics 365 Guides by using a QR code anchor, circular code anchor, or holographic anchor. This article shows how to anchor a guide with a QR code anchor. QR code anchoring is recommended because:

- You can use the QR code that comes with Dynamics 365 Guides or any other QR code that you already own.

- You can print the anchor in various sizes (but be sure to always use the same size for the same guide).

- You can embed a link to a guide (deep link) in a QR code. This makes it quicker for the operator to open the appropriate guide.

In certain cases, you may need to use a circular code or holographic anchor, however. [Learn about other types of anchors and when to use them](pc-app-anchor.md). 

> [!IMPORTANT]
> Anchoring a guide with a QR code requires HoloLens 2. This feature is not available on HoloLens 1.

## Overall process for creating a QR code anchor

The process of creating a QR code anchor involves four basic steps:

1. Use the **Anchor** wizard to select the QR code anchor method.

2. Print the anchor from the PDF file that the **Anchor** wizard creates.

3. Attach the anchor to a physical object in the real world.

4. Gaze at the anchor on [!include[pn-hololens](../includes/pn-hololens.md)] to anchor the guide.

## Set up a QR code anchor

You can access the **Anchor** wizard from the **Outline** page. The **Outline** page automatically appears after you create or open a guide.

1. On the **Outline** page, select **Set your anchor now**.

    ![Set your anchor now button](media/outline-page-3.PNG "Set your anchor now button")

2. On the **Choose an anchor method** page, select **Select** for the **QR Code** anchor method.

    ![Select button for the QR Code anchor method](media/qr-code-choose-method.PNG "Select button for the QR Code anchor method")

3. In step 1 of the wizard, select **Download QR code** to create a PDF file that is named **Guides-QRCodeAnchor**. This file includes the anchor that you will print in step 5.

    ![Download QR code button](media/qr-code-download-button.PNG "Download QR code button")

4. On your computer, open the **Guides-QRCodeAnchor** file.

5. Print the last page of the document on matte stock. (Glossy materials can affect scanning.) Bubble jet printers produce a better matte finish.

6. Make sure that the printed anchor measures between 101 and 400 millimeters (mm) wide. (These figures are based on [Version 1 QR code 
recommendations](https://www.qrcode.com/en/about/version.html).)

6. Attach the QR code anchor to a physical object in the real world, and then take a picture to help the operator find it.

7. Go back to the **Anchor** wizard in the PC app, and then select **Next** two times. (You can skip step 2 of the wizard if you took a picture of the anchor placement in the 
previous step.)

8. In step 3 of the wizard, select **Import** to import the picture that you took in step 6. Then drag it to the **Import anchor placement photo** box. When you've finished, 
select **Next** to move to the next step.

    ![Import button](media/qr-code-import-photo.PNG "Import button")

9. In step 4 of the wizard, if you want to change the default instructions for the operator, select **Edit step card text**, and then enter your instructions. When you've 
finished, select **Next** to move to the next step.

    ![Edit step card text button](media/qr-code-operator-instructions.PNG "Edit step card text button")

10. Put on your [!include[pn-hololens](../includes/pn-hololens.md)], open your guide, and then gaze at the QR code anchor to anchor the guide.

    ![Align HoloLens](media/qr-code-align-hololens.PNG "Align HoloLens")

## Best practices for QR code anchors

Keep the following points in mind when working with QR code anchors:

- **Printing settings**. Make sure to print the anchor on matte stock and don't laminate it.

    - Glossy materials can negatively affect scanning due to reflected light.
    
    - Bubblejet printers produce a better matte finish.

- **Size**.You can print QR codes in multiple sizes. For best detection and scanning comfort, we recommend printing the provided anchor with a width of 101 mm to 400 mm. This recommendation is for any QR code anchor following Version 1 QR codes. Anchor sizes outside of this recommended range might result in detection failure or reduced alignment precision for version 1 QR codes.

    > [!NOTE]
    > If you use your own QR code anchor, refer to QRCode.com for additional advanced QR code documentation. QR codes other than version 1 can increase the number of modules, which decreases their relative size. We recommend printing your anchor at a size where each independent module side measures a minimum of 3.5 mm.

- **Position**. Make sure that the anchor is always positioned flat. Do **not** distort it or place it on a curved surface. Otherwise, alignment and detection will be 
negatively affected.

- **Location**. Place the QR code anchor in a location that is easy to access, so it doesn't interfere with work and is easy to identify (for placement).

    - Ideally, anchor placement should be central to the steps that are being done.

    - Content that is placed farther away from the anchor will be subject to more position variability than content that is placed closer to it.

    - Place the anchor where operators can quickly re-scan it for realignment at any time, if required.

    - If operators must place/remove anchors before run-throughs, position variability of content will increase.

    - Ideally, the anchor should not be moved after the author places it. If a permanent placement isn't possible, consider creating a mount, so that the anchor can be placed 
    consistently in the same location/orientation each time.

    - Take a photo or video to document the anchor placement, and add it to the guide instructions. In this way, you can help increase operator confidence.

- **Orientation**. The way that you orient the anchor can have a big impact on scanning performance.

    - Position the anchor on a vertical surface to minimize light reflections, if possible.

    - Don't use reflective materials for the support surface.

    - Very reflective surfaces that are located behind the anchor, and direct exposure to sun or artificial light, can negatively affect scanning performance.

- **Scanning angle**. When you gaze at the anchor, make sure that you're facing it straight on and at the correct distance.

    - Scanning from glancing angles can cause detection failure or misalignment.

    - The ideal scanning range is from 50 to 150 centimeters (cm).

- **Contrast**. The brightness for the provided anchor is set to a 30-percent gray background. This setting provides the best adaptability for a wide variety of environments.

    - If you have trouble detecting an anchor that you provide, try to adjust the anchor's image brightness so that it matches the average environmental brightness around the 
    anchor.

