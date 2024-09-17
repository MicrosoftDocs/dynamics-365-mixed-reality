---
title: Annotate 2D snapshot in Dynamics 365 Remote Assist mobile
author: prashantyvr
description: Learn how to capture and annotate a 2D snapshot in the Dynamics 365 Remote Assist mobile app. 
ms.author: prashan
ms.date: 06/07/2024
ms.topic: article
ms.reviewer: v-wendysmith
---

# Capture and annotate snapshots in Dynamics 365 Remote Assist mobile 

Microsoft Dynamics 365 Remote Assist mobile users can capture and annotate a snapshot of their environment during a call. Users can then save the snapshot to their mobile device gallery, the in-call text chat, or both.

Snapshots are critical in situations where a still image might help communicate what a technician is looking at. Placing 2D annotations on snapshots provides emphasis on specific elements in the technician's environment. These snapshots can be used later for reference or work validation, and can help in low-bandwidth scenarios where live video isn't possible or on devices without augmented reality support. [Learn more about using snapshots in low-bandwidth scenarios](./poor-network-connectivity.md) and on [devices without augmented reality support](./calls-using-devices-without-AR.md). 

If the technician is using Dynamics 365 Field Service, they can also [post snapshots to an associated Dynamics 365 Field Service work order](./fs-integration.md).

> [!NOTE]
> Android devices that have a time-of-flight (ToF) sensor and support the [Depth API](https://developers.google.com/ar/discover/supported-devices) and iOS devices that have a LiDAR sensor [(see LiDAR sensor in the tables listed for iOS and iPadOS devices)](https://en.wikipedia.org/wiki/List_of_iOS_and_iPadOS_devices) are likely to have better accuracy with annotation placement.

## How it works

1. The technician selects the **Snapshot** button to snap a photo. 

    ![Screenshot with snapshot button highlighted.](./media/2D-snapshot-1.jpg "Screenshot with snapshot button highlighted")

    A **red border** appears on the technician's screen to indicate that the app is in Snapshot mode. The snapshot is automatically shared to the remote collaborator's screen on Microsoft Teams.

    ![Screenshot of the snapshot with the red border.](./media/2D-snapshot-2.jpg "Screenshot of the snapshot with the red border")

2. Both the technician and remote collaborator can place 2D annotations on the snapshot. 

    ![Screenshot of annotated snapshot.](./media/2D-snapshot-3.jpg "Screenshot of annotated snapshot")

3.	When the technician and remote collaborator are finished annotating the snapshot, the technician selects the **Check mark** button.  

    ![Screenshot showing highlighted Check mark button.](./media/2D-snapshot-4.jpg "Screenshot showing highlighted Check mark button")

4.	The technician is prompted to save the snapshot to the mobile device gallery, call chat, or both. 

    ![Screenshot of saving on snapshots.](./media/annotate-snapshots-1.jpg "Save snapshot")

5. The technician automatically returns to the live video call and can select the **Snapshot** button again to take more snapshots. 
   
    >[!NOTE] 
    > Annotations added to a snapshot do not appear in the technician's environment after the snapshot has been saved or discarded. 

6. If the technician successfully saves the snapshot, at the end of the call, the technician can view the snapshot in the mobile device gallery and/or Microsoft Teams text chat. 

    >[!NOTE] 
    > If the technician is using Dynamics 365 Field Service and saves their snapshot to the text chat, after the call ends, the technician can post their snapshots to an associated work order and view the snapshot there. [Learn more about Dynamics 365 Field Service integration](./fs-integration.md).
    > 
    > ![Screenshot of snapshots on Field Service work order.](./media/annotate-snapshots-2.jpg "Field Service")

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
