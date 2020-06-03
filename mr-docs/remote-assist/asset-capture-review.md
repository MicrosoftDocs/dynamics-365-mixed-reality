---
title: Review asset captures in Remote Assist UCI app
author: bencorn
description: Learn how to review captured asset data from the Remote Assist HoloLens app for validation purposes.
ms.author: becorn
ms.date: 5/30/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Review asset captures in Remote Assist UCI app

Captured asset data from the HoloLens is saved to Common Data Service (CDS) and viewable from the Remote Assist UCI app for validating work performed by technicians in the field, generating reports, and downloading artifacts like photos for use in other application.

In this article, you will learn how to access captured asset data through the Remote Assist UCI app and download that data to your computer.

## Prerequisites

To complete this article, you need:

- **Access to the environment Remote Assist is installed in**. You will access the Remote Assist UCI app to view asset data.

## View asset captures

1. From the main menu of your environment, select **Remote Assist** > **Assets** > and the asset you captured data to in the previous tutorial.
![Screenshot of the asset record list in Remote Assist web.](./media/06.19-asset-list.png "Remote Assist")
2. Select the **Captures** tab on the asset form to view the list of captures.
![Screenshot of the asset record form.](./media/06.20-asset-record.png "Remote Assist")
3. Select a capture record from the captures subgrid.
![Screenshot of the asset captures subgrid.](./media/06.21-asset-capture-list.png "Remote Assist")
4. Scroll down to view the image preview. The image can be expanded by selecting the **Full-screen view** button in the top right of the image preview control.
![Screenshot of the asset capture image preview.](./media/06.22-asset-capture-image-preview.png "Remote Assist")
5. Download the capture by selecting **Download** below the image preview control.
![Screenshot of the asset capture image preview.](./media/06.23-asset-capture-image-preview-expanded.png "Remote Assist")

## Next steps

In this tutorial, you learned how to view asset captures in the Remote Assist UCI app. To learn how to use Power Automate Flows to automate your business processes like generating reports with asset captures or notifying a Teams Channel when new asset data is captured, see:

> [!div class="nextstepaction"]
> [Automate asset capture data](./asset-capture-automation.md)