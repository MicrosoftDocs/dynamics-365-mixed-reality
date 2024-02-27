---
author: davepinch
description: Learn how to anchor holograms in the Microsoft Dynamics 365 Guides PC app by using a QR code anchor
ms.author: davepinch
ms.date: 02/27/2024
ms.topic: how-to
title: Anchor a guide in Dynamics 365 Guides by using a QR code anchor
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Anchor a guide in Dynamics 365 Guides by using a QR code anchor

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about creating a QR code anchor](https://youtu.be/NhdBG3emNUs)

Use a QR code anchor to anchor your guide to the real world in Guides. Review [best practices for QR code anchors.](pc-app-anchor-qr-best-practices.md) QR code anchoring is recommended because:

- You can use the [QR code that comes with Dynamics 365 Guides](qr-code-configuration.md) or any other QR code that you already own.

- You can print the anchor in various sizes (but be sure to always use the same size for the same guide).

- You can [embed a link to a guide in a QR code](pc-app-anchor-embed-qr-code-link.md). This makes it quicker for the operator to open the appropriate guide.

## Set up a QR code anchor

You can access the **Anchor** wizard from the **Outline** page in the PC app. The **Outline** page automatically appears after you create or open a guide.

1. On the **Outline** page, select **Set your anchor now**.

    ![Set your anchor now button.](media/outline-page-3.PNG "Set your anchor now button")

1. On the **Choose an anchor method** page, select **Select** for the **QR Code** anchor method.

1. In step 1 of the wizard, select **Download QR code** to create a PDF file that is named **Guides-QRCodeAnchor**. This file includes the anchor that you will print in step 5.

    ![Download QR code button.](media/qr-code-download-button.PNG "Download QR code button")

    You can use the same QR code for any guide that uses a QR code anchor.

1. On your computer, open the **Guides-QRCodeAnchor** file.

1. Print the last page of the document on matte stock. (Glossy materials can affect scanning.) Bubble jet printers produce a better matte finish.

1. Make sure that the printed anchor measures between 101 and 400 millimeters (mm) wide. (These figures are based on [Version 1 QR code recommendations](https://www.qrcode.com/en/about/version.html).)

1. Attach the QR code anchor to a physical object in the real world, and then take a picture to help the operator find it.

1. Go back to the **Anchor** wizard in the PC app, and then select **Next** two times. (You can skip step 2 of the wizard if you took a picture of the anchor placement in the previous step.)

1. In step 3 of the wizard, select **Import** to import the picture that you took. Then drag it to the **Import anchor placement photo** box. When you've finished, select **Next** to move to the next step.

   > [!TIP]
   > The filter is automatically set to **Images**, but you can change it.

    ![Import button.](media/qr-code-import-photo.PNG "Import button")

1. In step 4 of the wizard, if you want to change the default instructions for the operator, select **Edit step card text**, enter your instructions, and select **Save**. When you've finished, select **Next** to move to the next step.

    ![Edit step card text button.](media/qr-code-operator-instructions.PNG "Edit step card text button")

1. Put on your HoloLens, open your guide, and then gaze at the QR code anchor to anchor the guide.

## Next steps

- [Best practices for QR code anchors.](pc-app-anchor-qr-best-practices.md)
- [Guides QR code anchor configuration](qr-code-configuration.md)
- [Anchor a guide in the HoloLens app](hololens-app-anchor.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
