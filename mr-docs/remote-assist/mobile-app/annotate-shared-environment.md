---
title: Annotate the technician's environment in Dynamics 365 Remote Assist mobile
author: davepinch
description: How to add annotations to your environment in Dynamics 365 Remote Assist mobile 
ms.author: davepinch
ms.date: 04/04/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
---

# Annotate the technician's shared environment

[!INCLUDE [ra-teams-mobile-include](../../includes/ra-teams-mobile.md)]

In Microsoft Dynamics 365 Remote Assist mobile, mixed-reality annotations give technicians and remote collaborators the power to visually specify an area or a particular asset in their environment to look at or manipulate. During a Dynamics 365 Remote Assist mobile video call, the technician shares their environment with the remote collaborator through their rear-facing camera. The technician can instantly place mixed-reality annotations in the shared environment. The remote collaborator  places mixed-reality annotations on a snapshot of the technician's shared environment. 

> [!NOTE]
> Android devices that have a time-of-flight (ToF) sensor and support the [Depth API](https://developers.google.com/ar/discover/supported-devices) and iOS devices that have a LiDAR sensor [(see LiDAR sensor in the tables listed for iOS and iPadOS devices)](https://en.wikipedia.org/wiki/List_of_iOS_and_iPadOS_devices) are likely to have better accuracy with annotation placement.

## Learn the annotation tools

### Mobile app

If you're using the Dynamics 365 Remote Assist mobile app, you'll see the following annotation toolbar.

![Screenshot of the Dynamics 365 Remote Assist mobile annotation toolbar.](./media/mobile-app-annotation-toolbar.jpg "Screenshot of the Dynamics 365 Remote Assist mobile annotation toolbar")

If you select the down arrow next to the left-most button (the active tool), the button drops down. 

![Screenshot of the Dynamics 365 Remote Assist mobile annotation toolbar dropped down.](./media/mobile-app-annotation-toolbar-dropped-down.jpg "Screenshot of the Dynamics 365 Remote Assist mobile annotation toolbar dropped down")

The following table describes each of the buttons in the mobile app annotation toolbar.

|Button|Description|
|--------|-----------------------------------------------|
|![Screenshot of Arrow button.](./media/arrow-button-mobile.jpg "Screenshot of the Arrow button")|Add an arrow.|
|![Screenshot of Ink button.](./media/active-tool-button.jpg "Screenshot of Ink button")|Add ink (draw).|
|![Screenshot of Color picker button.](./media/color-picker-button.jpg "Screenshot of Color picker button")|Select a color for the annotation.|
|![Screenshot of Undo button.](./media/undo-button.jpg "Screenshot of Undo button")|Undo the last annotation that you placed in your environment.|
|![Screenshot of Delete all button.](./media/delete-all-annotations-button.jpg "Screenshot of Delete all button")|Delete all annotations that you placed in your environment. Note that you can't delete annotations placed by the remote collaborator.|

### Teams desktop app

If you're the remote collaborator and you're using Teams desktop, you'll see the following annotation toolbar.

![Screenshot of the Teams desktop annotation toolbar.](./media/teams-desktop-annotation-toolbar.jpg "Screenshot of the Teams desktop annotation toolbar")

The following table describes each of the buttons in the Teams desktop annotation toolbar.

|Button|Description|
|--------|-----------------------------------------------|
|![Screenshot of the Arrow button.](./media/arrow-button.jpg "Screenshot of the Arrow button")|Add an arrow.|
|![Screenshot of the Ink button.](./media/ink-button.jpg "Screenshot of the Ink button")|Add ink (draw).|
|![Screenshot of the Color picker button.](./media/color-picker-button.jpg "Screenshot of the Color picker button")|Select a color for the annotation.|
|![Screenshot of the Undo button.](./media/undo-button.jpg "Screenshot of the Undo button")|Undo the last annotation that you placed.|
|![Screenshot of the Delete all annotations button.](./media/delete-all-annotations-button.jpg "Screenshot of Delete all annotations button")|Delete all annotations that you placed during the session. Note that you can't delete annotations placed by the technician.|

### Add an arrow annotation 

1. Make sure the arrow is selected in the annotation toolbar. 

2. Move your device around to position the dot on the object or area you want to highlight.

3. Tap to place the ghost arrow on your device screen.

    ![Show ghost arrow in the Dynamics 365 Remote Assist mobile toolbar.](./media/share-annotation-1.jpg "RAM Ghost Arrow")

4. To rotate the arrow, tap and drag the arrow in a circular motion (360 degrees).

### Add an ink annotation 

1. Make sure the **Ink** tool is selected in the annotation toolbar.
 
2. Tap and drag on your screen to start drawing. 

## Add an annotation if you're a technician using Dynamics 365 Remote Assist mobile

- As a technician, you can place annotations in your shared environment. The remote collaborator will see your annotations in real time on their device.

    ![Screenshot of Dynamics 365 Remote Assist mobile showing an annotation.](./media/technician-11.jpg)

## Add an annotation if you're a remote collaborator using Dynamics 365 Remote Assist mobile

1. To add annotations, select **Start annotating**.    

    ![Remote collaborator on RAM single screen.](./media/share-annotation-3.jpg "RAM Remote Collaborator")
    
    > [!TIP]
    > To delete all annotations you add during an editing session, select the 
    ![Delete all annotations button.](./media/delete-all-annotations-button.jpg "Delete all annotations button") button.

2. You'll see a snapshot of the technician's environment. You can add your annotations to that snapshot.

     |Technician|Remote collaborator|
     |------------------------------------------------|------------------------------------------------|
     |![Screenshot of technician's mobile app screen.](./media/technician-11.jpg)|![Screenshot of remote collaborator's mobile app screen.](./media/remote-collaborator-11.jpg)| 

3. To stop adding annotations to the snapshot, select the **Check mark** button. You'll return to the technician's live video feed and your annotations will automatically appear in the technician's environment.

## Add an annotation if you're a remote collaborator using Teams desktop

1. To add annotations, select **Start editing**.

    ![Screenshot of the Start Editing option in the Microsoft Teams meeting toolbar.](./media/teams_2.png)

2. You'll see a snapshot of the technician's environment. You can add your annotations to the snapshot.

    |Technician|Remote collaborator|
    |----------------------------------|--------------------------------------------------------------------|
    |![Screenshot of the technician's mobile app screen.](./media/technician-12.jpg)|![Screenshot of the remote collaborator's Teams desktop screen.](./media/remote-collaborator-desktop-12.jpg)|    

3. To stop adding annotations to the snapshot, select **Stop editing**. You'll return to the technician's live video feed and your annotations will automatically appear in the technician's environment.

    ![Screenshot of a Microsoft Teams call window with emphasis on the stop editing button.](./media/teams_4.png)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
