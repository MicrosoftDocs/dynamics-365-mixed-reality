---
author: sophiasysun
description: Collaborate with a Remote Assist user via Microsoft Teams on mobile
ms.author: sopsun
ms.date: 02/17/2020
ms.service: crm-online
ms.topic: article
title: Collaborate with a Remote Assist user via Microsoft Teams on mobile
ms.reviewer: krbjoran
---

# Collaborate with a Remote Assist user via Microsoft Teams on mobile 

Dynamics 365 Remote Assist users and Microsoft Teams users can collaborate using a variety of devices to solve problems together, faster. Remote Assist is available on HoloLens and HoloLens 2, and also AR-capable iOS and Android mobile phones and tablets. Remote collaborators can use Microsoft Teams on PC or mobile to collaborate with Remote Assist users.

In this article, we'll explore how you can use Microsoft Teams on mobile to collaborate with a Remote Assist user. The benefit of using Teams on mobile (versus PC) is that you can collaborate with Remote Assist users on-the-go. 

When you use Teams on an Android or iOS device, you can collaborate in an ad hoc one-to-one call with one person who is using Remote Assist on HoloLens or HoloLens 2 ("Remote Assist HoloLens user"). You can also collaborate in an ad hoc one-to-one call with one person who is using Remote Assist on mobile ("Remote Assist mobile user"). For more information, visit our [article on requirements](requirements.md).

The features you can use to collaborate differ depending on whether you are collaborating with a Remote Assist HoloLens user or Remote Assist mobile user.

 Feature |  Available for Teams mobile user in a one-to-one call with one Remote Assist HoloLens user | Available for Teams mobile user in a one-to-one call with a Remote Assist mobile user 
---| ---| ---
Make outgoing call | Yes | Yes, but Remote Assist mobile user must have Remote Assist app open to be notified of the call.
Receive incoming call | Yes| Yes
Control outgoing video, outgoing audio, and incoming audio  | Yes | Yes
Annotate Remote Assist user’s environment using arrows and ink  | Yes | Yes
Annotate 2D snapshot using arrows and ink | No | Yes
Send a text message | Yes |Yes
Share files from OneDrive | Yes| Yes
Share photos from device | Yes | Yes
Record call | No; only the Remote Assist user can initiate the recording | No; only the Remote Assist user can initiate the recording
Share screen | Yes | No

## Make a call

Launch Teams and go to the **Calls** tab.

  ![Screenshot showing the calls icon in Teams.](media/TeamsMobile_Call.png)

Under **History**, you will see your recent contacts. Select one of the contacts to call them. 

## Use call controls
![Screenshot showing the call controls in Teams mobile.](media/TeamsMobile_CallControl.png "Call control")

Use call controls to specify whether your collaborator can see what you see, hear what you hear, and more.

Call controls are found at the bottom of the screen. 
- The **Video icon** controls outgoing video.
- The **Microphone icon** controls outgoing audio.
- The **Speaker icon** controls incoming audio.

For additional actions, select the ellipses icon. 

Regardless of whether you’re in a one-to-one call or a meeting with a Remote Assist HoloLens user, you can:
-	**Put the call on hold**
-	**Use dial pad**
-	**Toggle incoming video**
-	**Share your screen** – your screen will pop up as a video in the Remote Assist HoloLens user’s world.
-	**Start video with blur** (iOS only) - useful if you have sensitive information behind you or want to protect the privacy of colleagues who are behind you. 
- **Insert file** to display a file in the Remote Assist HoloLens user’s environment. The file can be from OneDrive, Teams, or it can be an image stored on your mobile device. Both you and the Remote Assist HoloLens user can view the files via Teams chat after the call ends. (You will notice that in a meeting, the call controls do not display an **Insert File** option. However, you can still display a file in the Remote Assist HoloLens user’s environment by using the **Share** feature).


> [!NOTE]
> Turn your phone horizonal to see more of the Remote Assist HoloLens user’s environment.   

## Annotate Remote Assist user’s environment

When you are in a call with a Remote Assist user, you will see their real world environment and holograms. 

To add an annotation, select the **Edit icon**.

Then, you will see the **Mixed Reality toolbar**. 

![Screenshot of the mixed reality toolbar, with the edit icon highlighted.](media/TeamsMobile_MRToolbar.png)

- To add arrows, select **Place arrow** (shown here: ![Graphic of the Place arrow icon in the mixed reality toolbar.](media/6584f4b7932378aa23f6efbf460b304c.png)). Then, tap where you would like to place the arrow. To control the direction of the arrow, tap, hold, and draw a circle with your finger until it is at the correct direction. Then release.

- To make drawing annotations, select the **Ink icon** (shown here: ![Graphic of the ink icon, as represented by a pencil.](media/187307e30fd713f5ae67aba854b78bc4.png)).

- To change the arrow or ink color, select the **Pick a color icon** (shown here: ![Graphic of the pick a color icon.](media/5d9d3c70cf19ed175a8dc1ad71a60fc5.png)). 
  
- To undo the most recent annotation you added, select **Undo**.

- To delete every annotation you’ve added, select **Erase** (shown here: ![Graphic showing the erase icon, which looks like a trash can.](media/3aab547aa81003ad181eceadc2c83a47.png)) and then select **Delete All Notes**.

- To delete only the annotations you added recently, select the **Erase icon** (shown here: ![Graphic showing the erase icon, which looks like a trash can.](media/3aab547aa81003ad181eceadc2c83a47.png)) and then select **Clear Current Notes**. It does not clear the annotations your collaborator added.

When you’re done adding annotations, select the checkmark icon to resume the live video feed. All annotations will persist even after you stopped editing. 

> [!NOTE]
> Each call participant can only undo and delete their own annotations.

## Send a text message

Select the **Text icon** (which looks like this: ![Graphic showing the text icon, which looks like a chat bubble.](media/TeamsMobile_Text.png)) to open the text chat and send text messages. After the call, all participants can access the messages (and OneDrive and Teams file links) via the Teams chat. 

> [!NOTE]
> You may notice that you can attach a photo, gif, or file via the text message. This is not the best way to share a file. We recommend sharing OneDrive file using this method and sharing a photo from your device using this method.

## Display OneDrive files

You can display a variety of OneDrive files in the Remote Assist HoloLens user's space. For example, add a PDF of a diagram to assist with the call so a technician or auditor can reference the diagram while keeping their head up and their hands free.

### Display and share link to OneDrive file  

Go to the call controls and select the ellipses icon [...]. Then select **Insert Files** and select whether to insert file from OneDrive or from Teams teams and channels.   

When you insert an image, still gif, video, or PDF from OneDrive or a Teams channel, it will show up as a new slate in the Remote Assist HoloLens user’s environment. A link to the file will be available in the Teams chat even after the call ends. (A link to the file will not appear in the Remote Assist chat.) 

The Remote Assist HoloLens user can save a file to their OneDrive by tapping the OneDrive icon in the top right of the slate. The OneDrive file is then automatically saved to a folder called "HoloLens Received Files."   

## Share files stored on your device

### Display and share link to on-device photo during a one-to-one call
Go to call controls and select the ellipses icon […]. Then select **Insert Files** and select **Photo**. Then, take a photo or select a photo from your mobile device’s photo gallery. 

Select the text chat. You'll see that the photo is attached to a blank message, but has not yet been sent. Send the photo.

![Screenshot of the photo option in Teams mobile.](media/TeamsMobile_SharePhoto.png "SharePhoto")

The photo will show up as a new slate in the Remote Assist HoloLens user’s environment and a link to the file will be available in the Teams chat even after the call ends. 

The Remote Assist HoloLens user can save a file to their OneDrive by tapping the OneDrive icon in the top right of the slate. The OneDrive file is then automatically saved to a folder on the HoloLens called "HoloLens Received Files."   

## Share your screen 

To share your screen, go to call controls, select the ellipses icon […], select **Share**, then select **Start Broadcast**.

![Screenshot of the Start broadcast window in Teams mobile.](media/TeamsMobile_ScreenBroadcast.png "ScreenBroadcast")

After a few seconds, a live view of your screen will be displayed as a new slate in the Remote Assist HoloLens user’s environment. 

### Share your screen in a meeting

![Screenshot of the share options in Teams mobile, including share screen.](media/TeamsMobile_ShareMultipleTypes.png "ShareMultipleTypes")

You have more options for sharing your screen in a meeting. Go to call controls and select the ellipses icon […]. Then, select one of the following options: Share photo, Share video, Share screen. (Share PowerPoint is not supported today). 

Share... | If you want to...
------------ | -------------
A photo | Take a photo to share or choose one from your gallery
Live video | Share live video from your camera
Your screen | Show your entire screen (within and outside the Teams app)



## What can Teams mobile users do in a one-to-one call with a Remote Assist mobile user? 

### Make outgoing calls

Launch Teams and go to the **Calls** tab.

  ![Screenshot of the Teams mobile calls action.](media/TeamsMobile_Call.png "Calls tab")

Under **History**, you'll see your recent contacts. Select one of the contacts to call them. 

> [!NOTE]
> A Remote Assist mobile user can only receive calls if they have Remote Assist app open.



### Use call controls

![Screenshot of the Teams mobile call controls](media/TeamsMobile_CallControl.png "Call control")

Use call controls to specify whether your collaborator can see what you see, hear what you hear, and control what you hear.

Call controls are found at the bottom of the screen. 
- Select the **video icon** to control outgoing video.
- Select the **microphone icon** to control outgoing audio.
- Select the  **speaker icon** to control incoming audio.

To use additional features, select the ellipses icon […].

Regardless of whether you’re in a 1:1 call or a meeting with a Remote Assist HoloLens user, you can:
- **Put the call on hold**
- **Use dial pad**
- **Toggle incoming video**
- **Share your screen** – your screen will pop up as a video in the Remote Assist HoloLens user’s world
- **Start video with blur** (iOS only) is useful if you have sensitive information behind you or want to protect the privacy of colleagues who are behind you. 



### Annotate Remote Assist user’s environment using arrows and ink   

When you're in a call with a Remote Assist user, you'll see their real world environment and holograms. 

To add an annotation, select the edit icon (represented by this icon: ![Graphic showing the pencil edit icon.](media/TeamsMobile_Edit.png)).

Then, you'll see the **mixed reality toolbar**. 

![Screenshot of the mixed reality toolbar](media/TeamsMobile_MRToolbar.png "MRToolbar")

- To add arrows, select **Place arrow** (represented by this icon: ![Graphic showing the place arrow icon.](media/6584f4b7932378aa23f6efbf460b304c.png)). Then, tap where you would like to place the arrow. To control the direction of the arrow, tap, hold, and draw a circle with your finger until it's at the correct direction. Then release.
- To add ink, select **Ink** (represented by this icon: ![Graphic showing the ink icon.](media/187307e30fd713f5ae67aba854b78bc4.png )).
- To change the arrow or ink color, select **Pick a color** (represented by this icon: ![Graphic showing the pick a color icon.](media/5d9d3c70cf19ed175a8dc1ad71a60fc5.png)).
- To undo the most recent annotation you added, select **Undo**.
- To delete every annotation you’ve added, select **Erase** (represented by this icon: ![Graphic showing the erase icon, which looks like a trash can.](media/3aab547aa81003ad181eceadc2c83a47.png)) and then select **Delete All Notes**.
- To delete only the annotations you added since the most recent time you entered Edit mode, select **Erase** (represented by this icon: ![Graphic showing the erase icon, which looks like a trash can.](media/3aab547aa81003ad181eceadc2c83a47.png)) and then select **Clear Current Notes**. Clearing current notes *does not* clear the annotations your collaborator added.

When you’re done adding annotations, select the check mark icon (represented here: ![Graphic showing the check mark icon.](media/TeamsMobile_Check.png "Check") to resume the live video feed. All the annotations you made will persist even after you stopped editing. 

> [!NOTE]
> Each collaborator can only delete their own annotations.

### Annotate 2D snapshot using arrows and ink

Remote Assist Mobile lets technicians take 2D snapshots of their environment and mixed reality annotations, and annotate them during a call. Snapshots are critical in situations where a still image might be needed to carefully add annotations to it. These snapshots can be used for reference later or work validation. Snapshots can also be utilized in low bandwidth situations.

When a Remote Assist mobile user sends a snapshot and starts annotating, their video feed will become a still video feed. Select **Start editing** to begin adding annotations. After both the technician and expert are finished annotating on the snapshot, the Remote Assist mobile user selects the check mark to exit from the annotation mode and can choose to save the snapshot to their phone’s photo gallery.

Annotations are only displayed during the snapshot session. When the Remote Assist mobile user exists snapshot mode, annotations will be removed. 

For more information, [learn more about using snapshots](./mobile-app/annotate-snapshot.md).

### Send a text message

Select the text chat (represented by this icon: ![Graphic showing the chat message icon.](media/TeamsMobile_Text.png "Text")) to open the text chat to send text messages. After the call, all participants can access the messages via the Teams chat.

### Share files

Use the the text chat (represented by this icon: ![Graphic showing the chat message icon.](media/TeamsMobile_Text.png "Text")) to attach a file.





