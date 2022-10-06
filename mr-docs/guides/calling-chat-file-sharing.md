---
title: 
author: 
description: 
ms.author: 
ms.date: 10/04/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Start a chat and share a file in Dynamics 365 Guides on HoloLens 

When a Microsoft Dynamics 365 Guides user on HoloLens is on a call with one or more remote collaborators on Microsoft Teams desktop, Microsoft Teams mobile, or Dynamics 365 Remote Assist, call participants can chat with each other, and the remote collaborator(s) on Teams or Dynamics 365 Remote Assist can share files or page links in the **Chat** window. This is particularly useful in service-related scenarios where the remote expert wants to share a diagram or some other illustration to help the Dynamics 365 Guides user diagnose and/or solve a problem. Participants can also share deep links to guides in a chat. For example, a Dynamics 365 Guides author might want to collaborate with a remote user by [sharing a direct link to a specific guide or even a step within a guide](pc-app-copy-link-guide-step.md).  

> [!NOTE]
> An adminstrator can remove the ability for a user to chat by modifying a Microsoft Teams policy. [Learn more about Teams policies supported by Dynamics 365 Guides](admin-teams-policies.md). File sharing for guest and external users is determined by Teams, OneDrive for Business, and SharePoint settings. [Learn more about guest access](admin-add-guest-user.md) 

## Start a chat from Dynamics 365 Guides

1. Select the **Chat** button to start a chat. 

    > [!NOTE]
    > If you receive a chat invite from a remote collaborator, a red circle appears on the **Chat** button and the **Chat** button animates. 

    ![Screenshot of Meetings window with Chat button highlighted.](media/calling-chat-file-sharing-1.JPG "Screenshot of Meetings window with Chat button highlighted")    
    
    A new **Chat** window appears to the right of the video feed.     
    
2. To respond to the chat, place your gaze cursor over the box that says "Type a new message". 

    ![Screenshot highlighting where to enter message.](media/calling-chat-file-sharing-3.JPG "Screenshot highlighting where to enter message")
    
3. In the holographic keyboard that appears, enter your message, or use the **Microphone** button to dictate a message. Select the **Send** button (or press the Return key on the holographic keyboard) when you're ready to send the message. 

    ![Screenshot showing holographic keyboard with Microphone button highlighted for dictation option.](media/calling-chat-file-sharing-4.JPG "Screenshot showing holographic keyboard with Microphone button highlighted for dictation option")
    
    If a remote collaborator shares a file or page link, the file or page automatically opens in a new window in your space. You can move this window wherever you want or size it directly with your hands. 

   ![Screenshot showing example file shared with the user.](media/calling-chat-file-sharing-5.JPG "Screenshot showing example file shared with the user")

   The remote collaborator can also paste a link into the **Chat** window to share a file.  
   
   > [!NOTE]
   > A remote collaborator can share a file with a Dynamics 365 Guides user, but the Dynamics 365 Guides user cannot share a file with other participants on the call.    
## Start a chat from Teams 

### Teams desktop (PC or Mac)

During a call with a Dynamics 365 Guides user, participants can communicate through text chat. The Dynamics 365 Guides user can only see messages that are exchanged during the call. The chat log is available through Teams after the call ends.

To start a chat:

1. In the call controls, select the **Chat** button. 

    ![Screenshot showing call controls with Chat button highlighted.](media/calling-teams-start-chat.JPG)    

2. To send a OneDrive or local file through chat, select the **Attach file** button or paste the file directly into the **Chat** window. 

    >[!Note]
    > Dynamics 365 Guides chat supports certain formats, including bold, italic, strikethrough, and underline. It also supports hyperlinks. However, it does not support HTML-formatted text or lists, such as a passage you copy and paste from a website. 
    >
    > For example, if you copy and paste text from a website that has HTML formatting and send it during a Dynamics 365 Guides call, the Dynamics 365 Guides user will see the plain text in the **Chat** window but the formatting may not be what you expect.

### Teams mobile

- Select the **Chat** button ![Graphic showing the Chat button.](media/calling-teams-mobile-start-chat.JPG) to open the text chat and send text messages. 

   After the call, all participants can access the messages (and OneDrive and Teams file links) via the Teams chat. 

## Share a file from Teams

A remote collaborator on Teams (PC, Mac, or mobile) can share a file when they're on a call with a Dynamics 365 Guides user on HoloLens. For example, a remote collaborator might want to share a .pdf file of a diagram to help the Dynamics 365 Guides user resolve a problem. The remote collaborator can share the following types of files: .jpg, .bmp, .png, .tif/.tiff, .pdf, still gif. 

To share a different type of file, for example, an instructional video or a series of instructions in a PowerPoint presentation, the remote collaborator can [share their desktop or application window](calling-screen-sharing.md). 

> [!NOTE]
> Dynamics 365 Guides follows Teams policies for sharing files. If your Teams policies are configured to prevent file sharing, users won't be able to share files with each other. See these links for more info:
>
> - [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access)
>
> - [Native chat experience for external (federated) users in Microsoft Teams](/microsoftteams/native-chat-for-external-users)

### Use Teams desktop (PC or Mac) to share a file 

You can share a OneDrive for Business file or a local file with a Dynamics 365 Guides user. Dynamics 365 Guides does not support sharing from a shared SharePoint folder or from a personal OneDrive folder. 

Use one of the following methods to share a file:

- In the **Mixed Reality** toolbar, select the **Add file** button. 

   ![Screenshot of Mixed Reality toolbar with Add file button highlighted.](media/calling-file-sharing-teams-desktop-mr-toolbar.JPG "SharePhoto") 

   The file will be uploaded to your OneDrive for Business folder and permissions to access that single file will be granted to all call participants.    

- In the Teams **Chat** window, select the **Attach file** button. 

- Copy and paste the file into the **Chat** window.

When you share a file, it appears as a new window in the Dynamics 365 Guides user's space and a link to the file is shared in the chat. All call participants can [annotate a file](calling-annotations.md) displayed in the Dynamics 365 Guides user's space. Note, however, that Teams mobile users can only annotate in one-to-one calls. 

> [!Note]
> After you share a file, you can't move, delete, or resize the file.

### Use Teams mobile to share a file 

#### Share a OneDrive for Business file 

> [!NOTE]
> Dynamics 365 Guides does not support sharing from a shared SharePoint folder or a personal OneDrive folder.   

1. In the call controls, select the **More info** button […].

    ![Screenshot of Call controls with More info button highlighted.](media/calling-file-sharing-mobile-call-controls.JPG "SharePhoto")

2. Select **Insert file**, and then select whether to insert the file from OneDrive for Business or from a Teams team or channel. You can insert an image, still gif, video, or .pdf file.

    The file appears as a new window in the Dynamics 365 Guides user’s environment. At this time, the Dynamics 365 Guides user cannot save the shared file in their own OneDrive for Business folder.

#### Share a photo from your phone 

1. In the call controls, select the **More info** button […].

    ![Screenshot of Call controls with More info button highlighted.](media/calling-file-sharing-mobile-call-controls.JPG "SharePhoto")

2. Select **Insert file**, and then select **Photo**. 

3. Take a photo or select a photo from your mobile device’s photo gallery. 

    ![Screenshot of the photo option in Teams mobile.](media/calling-file-sharing-photo-teams-mobile.JPG "SharePhoto")

4. Select the text chat. The photo is attached to a blank message. 

5. Send the photo.    

    The file appears as a new window in the Dynamics 365 Guides user’s environment. At this time, the Dynamics 365 Guides user cannot save the shared file in their own OneDrive for Business folder.

4. Select the text chat. The photo is attached to a blank message. 

5. Send the photo.    

## See also

- [Call a remote collaborator](calling-start-call.md)
- [Join a scheduled meeting](calling-meetings.md)
- [Record a call](calling-record-call.md)
- [Screen and file sharing](calling-screen-sharing.md)
- [Annotations](calling-annotations.md)
- [Access OneDrive files](onedrive-files.md)
- [Teams users capabilities](calling-teams-users.md)
- [Where call data is stored](call-logging.md)

    
