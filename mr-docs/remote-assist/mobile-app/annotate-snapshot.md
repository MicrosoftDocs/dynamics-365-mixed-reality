---
title: Annotate 2D snapshot in Dynamics 365 Remote Assist mobile
author: amaraanigbo
description: Learn how to capture and annotate a 2D snapshot in the Dynamics 365 Remote Assist mobile app. 
ms.author: soanigbo
ms.date: 04/13/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Capture and annotate snapshots in Dynamics 365 Remote Assist mobile 

Snapshots are critical in situations where a still image might help communicate what a technician is looking at. Placing 2D annotations on snapshots provides emphasis on specific elements in the technician's environment. These snapshots can be used later for reference or work validation, and can help in low-bandwidth scenarios where live video isn't possible or on devices without AR support. [Learn more about using snapshots in low-bandwidth scenarios](./poor-network-connectivity.md) and on [devices without augmented reality support](./calls-using-devices-without-AR.md). 

Dynamics 365 Remote Assist mobile users can capture and annotate snapshots of their environment during a call. Users can then save the snapshot to their mobile device gallery, the in-call text chat, or both.

If the technician is using Dynamics 365 Field Service, [snapshots can also be posted to an associated Dynamics 365 Field Service work order](./fs-integration.md).

## How it works

1. As the technician using Dynamics 365 Remote Assist mobile, select the **Snapshot** icon to snap your photo. 

    ![Screenshot of the snapshot icon in Dynamics 365 Remote Assist mobile.](./media/snapshot1.png "Snapshot Icon")

2. You'll know you're in snapshot mode when a **red border** appears on your device's screen. The snapshot is automatically shared to the remote collaborator's screen on Microsoft Teams.

    ![Screenshot of the snapshot icon with the red border.](./media/snapshot2.png "Red Border")

3. Both the technician and remote collaborator can place 2D annotations to the snapshot. 

    ![Screenshot of annotations on snapshots.](./media/snapshot4.png "Annotate snapshot")

4.	After both the technician and remote collaborator are finished annotating on the snapshot, the technician selects the **Check Mark** to **save** or **discard** the snapshot.  

    ![Screenshot of the check mark.](./media/snapshot4.png "Check Mark")

5.	The technician is prompted with the options to **discard** the snapshot or **save** the snapshot to either the **mobile device's photo gallery**, **Dynamics 365 Remote Assist mobile's text chat**, or **both**. Select your choice and then select **Save.**

    ![Screenshot of saving on snapshots.](./media/snapshot6a.png "Save snapshot")

6. The technician is notified when the snapshot has been **successfully saved** or **failed**. If the snapshot has not been saved, you can try taking another snapshot and saving it again. 

    ![Screenshot of successfully saving snapshots.](./media/snapshot7a.png "Saving snapshot success")

7. Afterwards, the technician is taken back to the live video call and can select the snapshot icon again to take more snapshots. 
   
    >[!NOTE] 
    > Annotations added on a snapshot will **not** appear in the technician's environment after it has been saved or discarded. 

8. If the technician successfully saved the snapshot, then the snapshots can be viewed in the **mobile device’s Photo Gallery** and/or **Microsoft Teams text chat** at the end of the call. 

9. If the technician is a Dynamics 365 Field Service customer and saved their snapshot to the text chat, after the call ends, the technician can post their snapshot(s) to an associated work order and view the snapshot there. Learn more about D365 Field Service integration [here](./fs-integration.md).

    ![Screenshot of snapshots on Field Service work order.](./media/12.png "Field Service")


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
