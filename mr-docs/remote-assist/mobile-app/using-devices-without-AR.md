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
# Using Remote Assist mobile on your mobile device without augmented reality (AR) support 

Technicians and remote collaborators can still connect and conduct repairs and inspections together on mobile devices **without** augmented reality (AR) support, too! Without a device with AR support, technicians and remote collaborators are unable to provide virtual annotations to the the real world as seen through the technician's device camera. However, technicians can still use the live video feed to share their environment and use the **snapshot feature** to provide instructions using 2D annotations along with the remote collaborator. Learn more about the snapshot feature, [here](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/mobile-app/annotate-snapshot). 

## Prerequisites 
- Technicians must be using a mobile device **without** AR support to follow along this guide. If your device is not listed on the [Android/ARCore](https://developers.google.com/ar/discover/supported-devices) supported devices or [iOS/ARKit](https://developers.google.com/ar/discover/supported-devices#ios) supported devices, then your device does not support AR. 
- Remote collaborators on Microsoft Teams desktop or mobile can use devices with or without AR support; this has no impact on the AR experience. 

## How it works 
1. The technician using on a mobile device without ARCore/ARKit support launches and signs into  Remote Assist. The technician selects **Sign In** and is taken to the **Contacts** page.

2. The technician is automatically notified that there will limited functionalities during a call because this mobile device does not support AR. The technician can dismiss this notification by selecting **Don't show again** or **Continue**.

3. The technician launches a call with a remote collaborator using Microsoft Teams desktop or mobile. The technician joins the video call **without** the Mixed Reality toolbar available and the remote collaborator joins the video call **without** both the “Edit” button and Mixed Reality toolbar available. 

4. The technician receives a tool tip notification directing the use of still snapshots to add 2D annotations on a frozen video frame. 

5. If the technician enters snapshot mode, this captures a frozen frame of technician’s environment and both the technician and remote collaborator can add 2D annotations to the snapshot. 
> [!NOTE]	Both the technician and remote collaborator will see the MR toolbar on the frozen frame and can add 2D annotations.

6. After both the technician and remote collaborator are finished annotating on the snapshot, the technician selects the Check Mark to save or discard the snapshot.

7. The technician is prompted with the options to discard the snapshot or save the snapshot to either the mobile device's Photo Gallery, Remote Assist mobile's text chat, or both. Select your choice(s) and then select Save.

8. The technican is notified when the snapshot has been successfully saved or failed. If the snapshot has not been saved, then you can try taking another snapshot and saving it again. If the technican successfully saved the snapshot, then the snapshots can be viewed in the mobile device’s Photo Gallery and/or Microsoft Teams text chat.

9. Afterwards, the technician is taken back to the live video call and can select the snapshot icon again to take more snapshots.
> [!NOTE] Annotations added on a still snapshot will not appear in the technician's environment after it has been saved or discarded.

10. The technician can send and receive messages, images, and files in the text chat from the remote collaborator. 

11. The technician can record the one-to-one call with the remote collaborator, if the remote collaborator is using Microsoft Teams desktop only. 

12. If the technician is a Dynamics 365 Field Service customer, at the end of the call the technician can choose to automatically post the call logs and the images, files, and snapshots shared in the text chat to an associated work order.

