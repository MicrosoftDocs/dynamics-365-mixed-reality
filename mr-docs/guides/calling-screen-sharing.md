---
title: 
author: 
description: 
ms.author: 
ms.date: 10/04/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Share your desktop or application screen with a Dynamics 365 Guides user on HoloLens

A remote collaborator on Microsoft Teams (PC, Mac, or mobile) can share their desktop or application screen to help a Dynamics 365 Guides user identify and/or resolve a problem. For example, the remote collaborator might want to share a video or a series of instructions in a PowerPoint presentation. 

For other types of files, the remote collaborator can share a file through Teams chat. The remote collaborator can share the following types of files through Teams chat: .jpg, .bmp, .png, .tif/.tiff, .pdf, still gif. 

This article shows how to share a screen with a Dynamics 365 Guides user. To learn how to share a file in a chat, see [Start a chat and share a file](calling-chat-file-sharing.md).

> [!NOTE]
> Dynamics 365 Guides follows Teams policies for sharing files. If your Teams policies are configured to prevent file sharing, users won't be able to share files with each other. See these links for more info:
>
> - [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access)
>
> - [Native chat experience for external (federated) users in Microsoft Teams](/microsoftteams/native-chat-for-external-users)

## Use Teams desktop (PC or Mac) to share a screen 

1. To share your desktop screen or an applicanon screen, select **Share**.

   ![Screenshot of the share tray button.](media/calling-screen-sharing-4.JPG "Screenshot of the Share tray button")
   
2. Select the application window you want to share, or share your desktop screen. 

    > [!Note]
    > You can share one application window or screen at a time. If you want to share a different screen, select the **Close share tray** button to stop sharing, select a different screen, and then start sharing again.

    The shared screen and the live video feed follow the behavior described later in this article.

## Use Teams mobile to share your screen 

1. In the call controls, select the **More info** button […].

    ![Screenshot of Call controls with More info button highlighted.](media/calling-file-sharing-mobile-call-controls.JPG "Screenshot of Call controls with More info button highlighted")

2. Select **Share**, and then select **Start Broadcast**.

    ![Screenshot of the Start broadcast window in Teams mobile.](media/calling-screen-sharing-5.JPG "Screenshot of the Start broadcast window in Teams mobile")

    After a few seconds, a live view of your screen will be displayed as a new window in the Dynamics 365 Guides user’s environment. 

    The shared screen and the live video feed follow the behavior described below.

## Work with a shared screen in Dynamics 365 Guides on HoloLens

When a remote collaborator shares their screen, the screen automatically appears as a new window in the Dynamics 365 Guides user's environment.

![Screenshot of a shared screen example in Dynamics 365 Guides on HoloLens.](media/calling-screen-sharing-1.JPG "Screenshot of a shared screen example in Dynamics 365 Guides on HoloLens")

The live video feed of the person sharing their screen is suspended in this case. The video feed and the shared screen cannot both be on at the same time.

You can use direct touch to move the shared screen around, and to size it. 

![Animation of moving screen around with direct touch.](media/Slate_NearInteractions.gif "Animation of moving screen around with direct touch")

You can also interact with the screen by using your gaze cursor. Using the gaze cursor is particularly useful for situations where you want to move the window further away from you. 

![Animation of moving screen around with far-field interactions.](media/Slate_FarInteractions.gif "Animation of moving screen around with far-field interactions")

If the video feed is switched to another person on the call while a screen is being shared, that person's video feed is displayed and the shared screen is suspended (turns gray). A button appears on the suspended screen that you can select to make the shared screen active again. 

![Screenshot of a suspended shared screen with button highlighted.](media/calling-screen-sharing-3.JPG "Screenshot of a suspended shared screen with button highlighted")

You can also make the shared screen active by selecting a similar button in the live video feed. 

![Screenshot of window with new live feed and button that you can use to switch back to the shared screen.](media/calling-screen-sharing-2.JPG "Screenshot of window with new live feed and button that you can use to switch back to the shared screen")

If you make the shared screen active by using either of these buttons, the video feed for the person displayed is suspended again. 

If the person who shared their screen stops sharing, the shared screen disappears, and the video feed for the person sharing their screen appears again. 

