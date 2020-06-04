---
title: Capture asset conditions with spatial markup
author: bencorn
description: How to capture asset conditions with spatial markup on HoloLens 2
ms.author: becorn
ms.date: 5/30/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Capture asset conditions with spatial markup in HoloLens 2

Remote Assist can be used to capture procedures and defects during jobs such as an inspection or while performing a repair. As an example, a technician can use Remote Assist on the HoloLens to capture photos of the equipment they are inspecting to highlight defects like wear and corrosion. The photos can then be viewed and downloaded from the Remote Assist UCI app by stakeholders within the organization, such as a service manager or site superintendent.

In this article, you will learn how to use the HoloLens 2 to view asset records created from the Remote Assist UCI app and capture photos of assets with spatial markup.

## Prerequisites

To complete this article, you need:

- **HoloLens 2**. The public preview requires a HoloLens 2 with Remote Assist installed. Ensure you have downloaded the latest update to Remote Assist through the Microsoft Store.
- **Access to the environment Remote Assist is installed in**. The account you sign into Remote Assist with needs access to the environment created in the first step and an active Remote Assist license.

## Capture asset conditions

### Enable the public preview

From Remote Assist, select **Settings** > **Preview Features**, and toggle the Asset Capture feature on. This step requires you to restart Remote Assist by closing the live tile and relaunching the app.

![Screenshot of the settings page in Remote Assist to enable preview features.](./media/08.01-settings-preview-features.png "Remote Assist")

> [!IMPORTANT]
> Enabling the public preview replaces the snapshot tool available from the in-call toolbar with the Asset Capture capabilities. This means photos taken in Remote Assist will be saved to Common Data Service and accessible through the Remote Assist model-driven app vs. OneDrive for Business. You can disable the preview on the HoloLens at any time by returning to Settings.

### View the asset list

Select the **Assets** tab. The list of assets entered through the Remote Assist UCI app are displayed in descending order by the last created date. At the bottom of the window, there is a search bar to search for assets by the **Name** field.

> [!NOTE]
> The **Assets** tab is also accessible during a call. As an example, while performing a real-time remote inspection, photos of the asset(s) being inspected can be captured to the asset record from the **Assets** tab.

### Capture photos with spatial markup

1. Select the **Assets** tab and then select an asset from the list. You can also use the search bar at the bottom of the window.
![Screenshot of the Assets tab in Remote Assist.](./media/06.05-assets-list.png "Remote Assist")
2. Select the ink or arrow tools to markup the asset in your environment. As an example, circling an area of corrosion on a pipe.
3. Enable the **Camera** tool to start capturing photos. The camera tool will remain enabled after taking a photo.
![Screenshot of the asset detail view in Remote Assist.](./media/06.14-asset.png "Remote Assist")
4. **Airtap** or say the **Snap** voice command to take a picture of the asset with the spatial markup. The photo will preview for several seconds and then be saved to Common Data Service.
![Screenshot of the camera mode enabled in Remote Assist.](./media/06.10-photo-ready.png "Remote Assist")

Any existing photo can be selected in the asset view to preview in the HoloLens environment. If the current user took the photo, they can also delete that photo in the preview window.

> [!NOTE]
> Captured photos are saved both locally to the HoloLens and to Common Data Service (CDS) where they're viewable from the Remote Assist UCI app.

## Next steps

In this tutorial, you learned how to view assets in the HoloLens and capture photos to the asset record with spatial markup. To learn how to review the captured data from the Remote Assist UCI app, see:

> [!div class="nextstepaction"]
> [Review asset captures](./asset-capture-review.md)