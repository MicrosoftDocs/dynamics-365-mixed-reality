---
title: Using the Dynamics 365 Remote Assist Mobile on non-AR capable devices 
author: xonatia
description: Guide for using Remote Assist mobile on non-AR devices
ms.author: xolee
ms.date: 05/28/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Using Remote Assist on a mobile device without augmented reality (AR) support

Technicians and remote collaborators can conduct repairs and inspections together and provide instructions using annotations, even if technicians are using mobile devices **without** augmented reality (AR) support! In these scenarios, technicians and remote collaborators are unable to provide instructions using 3D annotations on a live video feed. However, technicians can still share their **live video feed** of their environment and both the technicians and remote collaborators can provide instructions on **snapshots** using 2D annotations. Learn more about the snapshot feature, [here](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/annotate-snapshot). 

## Prerequisites 
- In order to follow along with this guide, technicians must be using a mobile device **without** AR support. If your device is not listed on the [Android/ARCore](https://developers.google.com/ar/discover/supported-devices) supported devices or [iOS/ARKit](https://developers.google.com/ar/discover/supported-devices#ios) supported devices, then your device does not support AR. 

## How it works 
1. As a technician using Remote Assist on a mobile device without ARCore/ARKit support, you can launch and sign in with your credentials. After you select **Sign In**, you will receive a notification about using a mobile device with augmented reality support.

![AR Notif](./media/2a.png "AR Notification")

2. After dismissing the notification, you will be taken to the **Contacts** page.

![Contacts](./media/2b.png "Contacts")

3. Select the remote collaborator you want to call and on the video card you can launch the call. 

![Video Card](./media/3a.png "Video Card")

4a. After the remote collaborator accepts the call, the technician will enter a video call. 
> [!NOTE]	Technicians cannot place Mixed Reality annotations on the live video feed, but they can on place annotations on the in-call snapshots.

![In call](./media/01.05-call-nonar.png "In call")

4b. The remote collaborator will see the technician's video feed. 
> [!NOTE]	Remote collaborators' cannot place Mixed Reality annotations on technicians' live video feed, but they can on place annotations on the in-call snapshots.

![Remote View](./media/3c-expert.png "Remote expert view in call")

5. The technician will receive a tool tip notification directing the use of still snapshots to add 2D annotations on a frozen video frame. 

![Tool tip](./media/01.05-call-nonar-1.png "Tool tip")

6a. After selecting the **snapshot** icon, the technician will enter snapshot mode, which captures a frozen frame of the technician's environment and shares it to the remote collaborator's screen. 

![Snapshot mode](./media/01.04-call-snapshot-preanno.png "Snapshot mode")

6b. The remote collaborator will see a frozen frame of the technician's video feed. 

![Remote view of Snapshot mode](./media/5-expert.png "Remote collab view of Snapshot mode")

7. Both the technician and remote collaborator can add 2D annotations to the snapshot. 
> [!NOTE]	Both the technician and remote collaborator will see the Mixed Reality toolbar on the frozen frame and can add 2D annotations.

![Snapshot mode](./media/01.03-call-snapshot-postanno.png "Snapshot mode")

8. After both the technician and remote collaborator are finished annotating on the snapshot, the technician selects the Check Mark to save or discard the snapshot.

![Snapshot mode](./media/01.04-call-snapshot-preanno.png "Snapshot mode")

9. The technician is prompted with the options to discard the snapshot or save the snapshot to either the mobile device's Photo Gallery, the text chat, or both. Select your choice(s) and then select **Save**.

![Save snapshot](./media/7a.png "Save snapshot")

10. If the technican successfully saved the snapshot to the text chat, then the snapshot can be viewed in the Remote Assist mobile's text chat and Microsoft Teams text chat.

![Saved in text chat?](./media/06.20-chat-image-portrait.png "Save successful?")

11. Afterwards, the technician is taken back to the live video call and can select the snapshot icon again to take more snapshots.
> [!NOTE] Annotations added on a still snapshot will **not** appear in the technician's environment after it has been saved or discarded.

12. Both the technician and remote collaborator can send and receive messages and share files + images from their local device in the text chat. Learn more about the file sharing feature [here](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/file-sharing).

![Text chat](./media/.png "Text chat")

13. Both the technician and remote collaborator can record the one-to-one Remote Assist call, if the remote collaborator is using Microsoft Teams desktop only. The recording will be saved to Microsoft Stream and the link to the reocrding will be sent to the Microsoft Teams text chat. Learn more about the call recording feature [here](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/call-recording).

![Recording](./media/11b.png "Recording")

14. If the technician is a Dynamics 365 Field Service customer, at the end of the call, the technician can choose to automatically post the call logs and the images, files, and snapshots shared in the text chat to an associated work order. Learn more about Field Service integration [here](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/fs-integration).

![Field Service](./media/12.png "Field Service")
