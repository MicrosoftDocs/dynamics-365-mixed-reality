---
title: Call another Dynamics 365 Remote Assist mobile user from Dynamics 365 Remote Assist mobile
author: amaraanigbo 
description: Learn how calling between two Dynamics 365 Remote Assist mobile users works
ms.author: soanigbo
ms.date: 02/01/2023
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Call another Dynamics 365 Remote Assist mobile user from Dynamics 365 Remote Assist mobile

Technicians using Microsoft Dynamics 365 Remote Assist mobile can call and collaborate with their peers who are also using Dynamics 365 Remote Assist mobile. This article shows how to do one-to-one calls. See the following articles for different mobile app scenarios:

- [Collaborate with colleagues on Microsoft Teams desktop or Teams mobile](remote-assist-mobile-to-teams-calls.md)
- [Participate in group calls](group-calling.md)


## Prerequisites

- Call receivers with an iOS mobile device must **not** have the Microsoft Teams application on the device. Call receivers with an Android mobile device must choose Remote Assist Mobile for answering calls by [disabling Teams Mobile call notifications](remote-assist-mobile-to-teams-calls.md#what-happens-when-dynamics-365-remote-assist-mobile-and-teams-mobile-are-installed-on-the-same-device). 

- Technicians must have a Dynamics 365 Remote Assist [free trial](../try-remote-assist.md) or [subscription](../buy-remote-assist.md).

- Remote collaborators must have a Dynamics 365 Remote Assist free trial or subscription and a Microsoft Teams [free trial or subscription](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software). Learn how to set up Dynamics 365 Remote Assist with [Teams desktop](../teams-pc-all.md) and [Teams mobile](../teams-mobile-all.md).

## Call another Dynamics 365 Remote Assist mobile user

1. Launch and sign in to Dynamics 365 Remote Assist on your iOS or Android phone or tablet.

1. Search for the remote collaborator's name.

    ![Screenshot of Dynamics 365 Remote Assist mobile, showing the contacts screen and highlighting the search icon.](./media/ram-to-ram-search-collaborator.jpg "Search")

1. Select the remote collaborator's name, and then select **Launch Call**.

    ![Screenshot of Dynamics 365 Remote Assist mobile showing the Launch Call button.](./media/ram-to-ram-launch-call.jpg)

   > [!NOTE]
   > If the remote collaborator is receiving the call on an iOS mobile device with both Dynamics 365 Remote Assist mobile and Teams mobile installed, the remote collaborator can only answer on Teams mobile.

1. If the remote collaborator answers the call on **Remote Assist mobile**, the technician's live video feed is shared to the remote collaborator's device screen.

     |Technician|Remote collaborator|
     |------------------------------------------------|------------------------------------------------|
     |![Screenshot of the technician's mobile app call.](./media/technician-toolbar.jpg)|![Screenshot of the remote collaborator's mobile app call.](./media/remote-collaborator-toolbar.jpg)|    

1. If the remote collaborator wants to share their own environment, the remote collaborator can select the **More** button, and then select **Start sharing space and annotations**.

    ![Screenshot of switching environment on Dynamics 365 Remote Assist mobile to Dynamics 365 Remote Assist mobile calls.](./media/share-space-annotations.jpg)

1. When the remote collaborator starts sharing their space, the technician can view the remote collaborator's space by selecting **Switch view**.

    ![Screenshot showing notification that someone is sharing.](./media/ram-to-ram-switch-view.jpg "View others' space")

1. Either call participant can place annotations directly in the shared environment (their own environment) or by selecting **Start annotating**. 

    > [!NOTE] 
    > After the remote collaborator selects **Start annotating**, they can add mixed-reality annotations on a frozen frame of the shared environment. When they select the **Check mark** button, the annotation appears in the technician's shared environment.

     |Technician|Remote collaborator|
     |------------------------------------------------|------------------------------------------------|
     |![Screenshot of the technician's mobile app screen.](./media/technician-toolbar-2.jpg)|![Screenshot of the remote collaborator's mobile app screen showing the Start annotating command.](./media/remote-collaborator-2-toolbar.jpg)|  

1. The technician can use the call controls toolbar to change between a video call and audio-only call, mute or unmute their microphone, turn the speaker on or off, or end the call. 

    ![Screenshot of the Dynamics 365 Remote Assist call controls toolbar.](./media/call-controls-1.jpg)
    
    Selecting the **More** button from the call controls toolbar enables the technician to add participants, share their space and annotations, share their screen, or record the call.
    
    ![Screenshot of the Dynamics 365 Remote Assist call controls toolbar with More button highlighted and opened.](./media/call-controls-more-menu.jpg)

1. During the call, participants can capture and annotate on snapshots, send messages, share files, and more.

[!INCLUDE[footer-include](../../includes/footer-banner.md)]
