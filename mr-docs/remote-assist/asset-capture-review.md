---
title: Review data from captured assets in the Dynamics 365 Remote Assist model-driven app
author: prashantyvr
description: Learn how to review captured asset data from the Dynamics 365 Remote Assist HoloLens app for validation purposes.
ms.author: prashan
ms.date: 06/07/2024
ms.topic: article
ms.reviewer: v-wendysmith
---

# Review data from asset captures in the Dynamics 365 Remote Assist model-driven app

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

Captured asset data from the HoloLens app is saved to Microsoft Dataverse. From there, the data can be viewed from the Microsoft Dynamics 365 Remote Assist model-driven app for validating work performed by technicians in the field, generating reports, and downloading artifacts like photos or videos for use in other applications.

In this tutorial, you'll learn how to access captured asset data through the Dynamics 365 Remote Assist model-driven app and download that data to your computer.

## Prerequisites

To complete this tutorial, you need:

- **Access to the environment Dynamics 365 Remote Assist is installed in**. You'll access the Dynamics 365 Remote Assist model-driven app to view asset data.

## View asset captures

1. From the main menu of your environment, select **Remote Assist** > **Assets**, and then select an existing asset.

    ![Screenshot of the asset record list in Dynamics 365 Remote Assist.](./media/06.19-asset-list.png "Screenshot of the asset record list in Dynamics 365 Remote Assist")

2. Select the **Attachments** tab on the asset form.

    ![Screenshot of the asset record form.](./media/06.20-asset-record.png "Screenshot of the asset record form")

3. Select a capture record from the captures subgrid.

    ![Screenshot of the asset capture subgrid.](./media/06.21-asset-capture-list.png "Screenshot of the asset capture subgrid")

4. Scroll down to view the image preview. The image can be expanded by selecting the **Full-screen view** button in the upper-right corner of the image preview control.

    ![Screenshot of the asset capture image preview.](./media/06.22-asset-capture-image-preview.png "Screenshot of the asset capture image preview")

5. The image can be annotated by drawing directly on the image with your mouse. This is helpful for calling attention to objects or defects in the scene.

    ![Screenshot of an annotated image capture.](./media/06.27-asset-capture-image-preview-annotated.png "Screenshot of an annotated image capture")

6. Captures can be downloaded by selecting **Download** below the image preview control.

    ![Screenshot of the asset capture image download.](./media/06.23-asset-capture-image-preview-expanded.png "[Screenshot of the asset capture image download")

7. Quickly switch between captures by selecting the **Open Record set** button to the left of the **Save** button. The captures related to the asset appear on the left.

    ![Screenshot of the open record set control.](./media/06.28-asset-capture-switcher.png "Screenshot of the open record set control")

## Next step

In this tutorial, you learned how to view asset captures in the Dynamics 365 Remote Assist model-driven app. Next, learn how to use Power Automate flows to automate your business processes, like generating reports with asset captures or sending an email notification when new asset data is captured.

> [!div class="nextstepaction"]
> [Automate asset capture data](./integrate-power-automate.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
