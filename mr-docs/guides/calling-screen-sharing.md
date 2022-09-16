---
title: 
author: 
description: 
ms.author: 
ms.date: 10/04/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Share a file or screen with a Dynamics 365 Guides user on HoloLens

A remote collaborator on Microsoft Teams (PC, Mac, or mobile) can share a file or their screen when they're on a call with a Dynamics 365 Guides user on HoloLens. For example, a remote collaborator might want to share a .pdf file of a diagram to help the Dynamics 365 Guides user resolve a problem.

- **When to share a file**. The remote collaborator can share a file for the following file types: .jpg, .bmp, .png, .tif/.tiff, .pdf, still gif.

- **When to share a desktop or application window**. To share a different type of file, for example, an instructional video or a series of instructions in a PowerPoint presentation, the remote collaborator can share their desktop or application window. 

This article shows how to share a file or screen with a Dynamics 365 Guides user. The article also describes the behavior of a shared screen. 

> [!NOTE]
> Dynamics 365 Guides follows Teams policies for sharing files. If your Teams policies are configured to prevent file sharing, users won't be able to share files with each other. See these links for more info:
>
> - [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access)
>
> - [Native chat experience for external (federated) users in Microsoft Teams](/microsoftteams/native-chat-for-external-users)

## Use Teams (PC or Mac) to share a file with a Dynamics 365 Guides user on HoloLens

You can share a OneDrive file or a local file with a Dynamics 365 Guides user.   

Use one of the following methods to share a file:

- In the **Mixed Reality** toolbar, select **Add file** to share a file from OneDrive or your computer. 

   ![Screenshot of Mixed Reality toolbar with Add file button highlighted.](media/calling-file-sharing-teams-desktop-mr-toolbar.JPG "SharePhoto") 

   The file will be uploaded in your personal OneDrive and permissions to access that single file will be granted to all call participants.    

- In the Teams Chat window, select **Attach file** to share a file from OneDrive or your computer. 

When you share a file, it appears as a new window in the Dynamics 365 Guides user's space and a link to the file is shared in the chat. All call participants can [annotate a file](calling-annotations.md) displayed in the Dynamics 365 Guides user's space.

> [!Note]
> After you share a file, you can't move, delete, or resize the file.

## Use Teams mobile to share a file with a Dynamics 365 Guides user on HoloLens

### Share a OneDrive file 

1. In the call controls, select the **More info** button […].

    ![Screenshot of Call controls with More info button highlighted.](media/calling-file-sharing-mobile-call-controls.JPG "SharePhoto")

2. Select **Insert file**, and then select whether to insert the file from OneDrive or from a Teams team or channel. You can insert an image, still gif, video, or .pdf file.

    The file is uploaded to OneDrive and appears as a new window in the Dynamics 365 Guides user’s environment. The Dynamics 365 Guides user can save the file to their OneDrive by selecting the **OneDrive** button in the upper-right corner of the window. The OneDrive file is then saved to a folder called "HoloLens Received Files." A link to the file is available in the Teams chat after the call ends.

### Share a photo from your phone 

1. In the call controls, select the **More info** button […].

    ![Screenshot of Call controls with More info button highlighted.](media/calling-file-sharing-mobile-call-controls.JPG "SharePhoto")

2. Select **Insert file**, and then select **Photo**. 

3. Take a photo or select a photo from your mobile device’s photo gallery. 

    ![Screenshot of the photo option in Teams mobile.](media/calling-file-sharing-photo-teams-mobile.JPG "SharePhoto")

4. Select the text chat. The photo is attached to a blank message. 

5. Send the photo.    

    The file is uploaded to OneDrive and appears as a new window in the Dynamics 365 Guides user’s environment. The Dynamics 365 Guides user can save the file to their OneDrive by selecting the **OneDrive** button in the upper-right corner of the window. The OneDrive file is then saved to a folder called "HoloLens Received Files." A link to the file is available in the Teams chat after the call ends.

## Use Teams (PC or Mac) to share a screen with a Dynamics 365 Guides user on HoloLens

1. To share a screen of your desktop or a running application, select **Share**.

   ![Screenshot of the share tray button.](media/calling-screen-sharing-4.JPG "Screenshot of the Share tray button")
   
2. Select the application window you want to share, or share your desktop screen. 

    > [!Note]
    > You can share one application window or screen at a time. If you want to share a different screen, select the **Close share tray** button to stop sharing, select a different screen, and then start sharing again.

    The shared screen and the live video feed follow the behavior described later in this article.

## Use Microsoft Teams mobile to share your screen with a Dynamics 365 Guides user on HoloLens

1. In the call controls, select the **More info** button […].

    ![Screenshot of Call controls with More info button highlighted.](media/calling-file-sharing-mobile-call-controls.JPG "Screenshot of Call controls with More info button highlighted")

2. Select **Share**, and then select **Start Broadcast**.

    ![Screenshot of the Start broadcast window in Teams mobile.](media/calling-screen-sharing-5.JPG "Screenshot of the Start broadcast window in Teams mobile")

    After a few seconds, a live view of your screen will be displayed as a new window in the Dynamics 365 Guides user’s environment. 

    The shared screen and the live video feed follow the behavior described below.

## Work with a shared screen in Dynamics 365 Guides on HoloLens

When a remote collaborator shares their screen, the screen automatically appears as a new window in the Dynamics 365 Guides user's environment.

![Screenshot of a shared screen example in Dynamics 365 Guides on HoloLens.](media/calling-screen-sharing-1.JPG "Screenshot of a shared screen example in Dynamics 365 Guides on HoloLens")

The live video feed of the person sharing their screen is suspended in the Meeting window in this case. The video feed and the shared screen cannot both be on at the same time.

You can use direct touch to move the shared screen around, and to size it. You can also interact with the screen by using your gaze cursor. Using the gaze cursor is particularly useful for situations where you want to move the window further away from you. 

If the video feed is switched to another person on the call while a screen is being shared, that person's video feed is displayed in the Meeting window and the shared screen is suspended (turns gray). A button appears on the suspended screen that you can select to make the shared screen active again. 

![Screenshot of a suspended shared screen with button highlighted.](media/calling-screen-sharing-3.JPG "Screenshot of a suspended shared screen with button highlighted")

You can also make the shared screen active by selecting a similar button in the live video feed in the Meeting window. 

![Screenshot of Meeting window with new live feed and button that you can use to switch back to the shared screen.](media/calling-screen-sharing-2.JPG "Screenshot of Meeting window with new live feed and button that you can use to switch back to the shared screen")

If you make the shared screen active by using either of these buttons, the video feed for the person displayed in the Meeting window is suspended again. 

If the person who shared their screen stops sharing, the shared screen disappears, and the video feed for the person sharing their screen appears in the Meeting window again. 

