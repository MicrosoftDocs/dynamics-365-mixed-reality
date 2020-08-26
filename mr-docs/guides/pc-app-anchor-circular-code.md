---
author: Mamaylya
description: Learn how to anchor holograms in the Microsoft Dynamics 365 Guides PC app by using a circular code anchor
ms.author: mamaylya
ms.date: 10/01/2020
ms.service: crm-online
ms.topic: article
title: Anchor a guide in the Dynamics 365 Guides PC app by using a circular code anchor
ms.reviewer: v-brycho
---

# Anchor a guide in the Dynamics 365 Guides PC app by using a circular code anchor 

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about creating a circular code anchor](https://aka.ms/guidesprintedanchor)

You can anchor your guide to the real world in Microsoft Dynamics 365 Guides by using a QR code anchor, circular code anchor, or holographic anchor. This article shows how to anchor a guide with a circular code anchor. [Learn about other types of anchors and when to use them](pc-app-anchor.md).

## Overall process for creating a circular code anchor

The process of creating a circular code anchor involves four basic steps:

1. Use the **Anchor** wizard to select the circular code anchor method.

2. Print the anchor from the PDF file that the **Anchor** wizard creates.

3. Attach the anchor to a physical object in the real world.

4. Gaze at the anchor on [!include[pn-hololens](../includes/pn-hololens.md)] to anchor the guide.

## Set up a circular code anchor

You can access the **Anchor** wizard from the **Outline** page. The **Outline** page automatically appears after you create or open a guide.

1. On the **Outline** page, select **Set your anchor now**.

    ![Set your anchor now button](media/outline-page-3.PNG "Set your anchor now button")

2. On the **Choose an anchor method** page, select **Select** for the **Circular Code** anchor method.

    ![Select button for the Circular Code anchor method](media/circular-code-choose-method.PNG "Select button for the Circular Code anchor method")

3. In step 1 of the wizard, select **Download circular code** to create a PDF file that is named **Guides-CircularCodeAnchor**. This file includes the anchor that you will 
print in step 6.

    ![Download circular code button](media/circular-code-download-code.PNG "Download circular code button")

4. On your computer, in Adobe Acrobat Reader, open the **Guides-CircularCodeAnchor** file.

    > [!IMPORTANT]
    > [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] supports one size of circular code anchor. To ensure the best possible alignment accuracy, it's crucial 
    that you print the anchor at the specified size. If you use Adobe Acrobat Reader, you can set the specified size to get the best printing results.

5. Select **File** \> **Print**, and then, under **Page Sizing & Handling**, select the **Actual size** option.

    ![Actual size option](media/adobe-actual-size.PNG "Actual size option")

6. Print the last page of the document on matte stock. (Glossy materials can affect scanning.) Bubble jet printers produce a better matte finish.

7. Make sure that the printed marker spacing matches the measurements that are shown in the following illustration.

    ![Circular code anchor measurements](media/circular-code-measurements.PNG "Circular code anchor measurements")

    > [!NOTE]
    > If the anchor spacing isn't within +/– 0.1 mm, in the **Print** dialog box, select the **Custom Scale** option, and then change the percentage to compensate for the 
    size discrepancy. For example, if the result is 49 mm when you print the anchor, change the scale to 100.4 percent to get 49.196 mm, which is within tolerance.

8. Attach the circular code anchor to a physical object in the real world, and then take a picture to help the operator find it.

9. Go back to the **Anchor** wizard in the PC app, and then select **Next** two times. (You can skip step 2 of the wizard if you took a picture of the location in the previous 
step.)

10. In step 3 of the wizard, select **Import** to import the picture that you took in step 8. Then drag it to the **Import anchor placement photo** box. When you've finished, 
select **Next** to move to the next step.

    ![Import button](media/circular-code-import-photo.PNG "Import button")

11. In step 4 of the wizard, if you want to change the default instructions for the operator, select **Edit Step card text**, and then enter your instructions. When you've 
finished, select **Next** to move to the next step.

    ![Edit Step card text button](media/circular-code-operator-instructions.PNG "Edit Step card text button")

12. Put on your [!include[pn-hololens](../includes/pn-hololens.md)], open your guide, and then gaze at the circular code anchor to anchor the guide.

    ![Align HoloLens](media/circular-code-align-hololens.PNG "Align HoloLens")

## Best practices for circular code anchors

Keep the following points in mind when you work with circular code anchors:

- **Material surface.** Be sure to print the anchor on matte stock, and don't laminate it. Glossy materials can negatively affect scanning because of reflected light. Also, 
make sure that the anchor is flat. An anchor that is curved or distorted can affect alignment and detection.

- **Same anchor for authoring and printing.** For the best accuracy, use the same circular code anchor for authoring and operating.

- **Size.** Make sure that your circular code anchor is the exact size that is indicated in this topic. Incorrect anchor size causes misalignment of the guide.

    - Some applications and printers might change the size of the image.

    - If the anchor is larger than indicated, [!include[pn-hololens](../includes/pn-hololens.md)] interprets the scale difference in distance. Therefore, the anchor is 
    identified as closer than it really is.

    - The best way to make sure that the anchor isn't resized is to print it from the PDF file, as described earlier in this topic.

- **Location.** Place the anchor in a location on the physical object that is easy to access and out of the way.

    - Ideally, the anchor placement should be central to the steps that are being performed.

    - Content placed farther away from the anchor will be less accurate.

    - Place the anchor where operators can quickly rescan to realign at any time.

    - Ideally, the anchor should not be moved after the author places it. If a permanent placement isn't possible, consider creating a mount, so that the anchor can be 
    consistently placed in the same location/orientation every time.

    - Take a photo or video to document the circular code anchor placement, and add it to the guide instructions. In this way, you can help increase operator confidence. For 
    information about how to capture a photo or video from [!include[pn-hololens](../includes/pn-hololens.md)], see 
    [Mixed reality capture](https://docs.microsoft.com/windows/mixed-reality/mixed-reality-capture).

- **Scanning angle.** Make sure you're facing the anchor straight on at the correct distance when gazing at it. 

    - Scanning from glancing angles can cause detection failure or misalignment.

    - Ideal scanning range is from 60 to 80 cm.


