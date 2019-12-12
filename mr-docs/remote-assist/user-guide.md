---
author: sophiasysun
description: Dynamics 365 Remote Assist user guide (for HoloLens)
ms.author: sopsun
ms.date: 10/16/2019
ms.service: crm-online
ms.topic: article
title: Dynamics 365 Remote Assist user guide (for HoloLens)
ms.reviewer: v-brycho
---

# Dynamics 365 Remote Assist user guide (for HoloLens)

Use [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] to connect and collaborate using
hands-free video calling, mixed reality annotations, and file (image and PDF)
sharing. Use your [!include[pn-hololens](../includes/pn-hololens.md)] to call an expert who's using [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-teams](../includes/pn-teams.md)], and
then share what you see on [!include[pn-hololens](../includes/pn-hololens.md)] to solve problems and complete tasks
together, faster.

Need more help? [Check out Dynamics 365 Remote Assist FAQ](faq.md) for answers to common questions.

[Watch how-to videos](videos.md) about [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)].

## What you’ll need

-   A subscription to [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)]. [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] is included in the [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] subscription for individuals using a [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] license on [!include[pn-HoloLens](../includes/pn-HoloLens.md)]. A [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] license is also required for individuals (experts) who communicate with a [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] user on [!include[pn-HoloLens](../includes/pn-HoloLens.md)]. [!include[pn-teams](../includes/pn-teams.md)] may be available [as a free download](https://teams.microsoft.com/downloads) for these users. If you’re the admin for your organization, [learn how to try or buy, and deploy Dynamics 365 Remote Assist](../licensing/buy-and-deploy.md). 

    > [!TIP] 
    > You can try [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] for free for up to 90 days. [Learn more about the free 90-day Dynamics 365 Remote Assist trial](try-remote-assist-free.md).

-   A [HoloLens running the Windows 10 April 2018
    Update](https://support.microsoft.com/help/12643).

-   To make a video call, you'll need a contact using the latest version of [Microsoft
    Teams](https://products.office.com/microsoft-teams/group-chat-software) on
    a PC running [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 or a mobile device running [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] Mobile. [Learn about using Teams with
    Dynamics 365 Remote Assist.](use-microsoft-teams-with-remote-assist.md)

-   To connect to [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] from within [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)],
    you’ll need a [Dynamics 365 license](https://dynamics.microsoft.com/field-service/overview/?&OCID=AID720979_SEM_yeaT05hp&lnkd=Bing_D365_Brand).

-   An internet connection. At least 1.5 MB of bandwidth is recommended for the
    best experience.

Need to get up to speed on [!include[pn-hololens](../includes/pn-hololens.md)]? [Get help](https://support.microsoft.com/products/hololens).

## Install the Dynamics 365 Remote Assist app

How you install [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] depends on how your administrator chooses to
distribute the app. Your admin might have you [install the app from the Microsoft
Store for Consumers](https://www.microsoft.com/store/apps/9P77QGW10K9M), from your organization’s private store, through an email
link, or another method.

### Install the application through the Microsoft Store for Consumers

1.  On your [!include[pn-hololens](../includes/pn-hololens.md)], go to **Start** ![Start](media/d2a2ae5e90bdd0e0642abb5458af1016.png "Start") \> **[!include[cc-microsoft](../includes/cc-microsoft.md)] Store** ![[!include[cc-microsoft](../includes/cc-microsoft.md)] Store](media/2ac602b5a7855d312f3e7d924732acca.png "Microsoft Store"), and then search for “[!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)].”

2.  On your [!include[pn-hololens](../includes/pn-hololens.md)], go to **Start** ![Start](media/d2a2ae5e90bdd0e0642abb5458af1016.png "Start") \> **All apps**. Select **[!include[pn-remote-assist](../includes/pn-remote-assist.md)]**, then select it again to launch the app. [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] is an immersive app with a [holographic view](https://support.microsoft.com/help/12635), so it will be the only app you see while you’re using it.

If your [!include[pn-hololens](../includes/pn-hololens.md)] is running the April 2018 Update and you're signed in with an
[!include[pn-azure-active-directory](../includes/pn-azure-active-directory.md)] ([!include[pn-azure](../includes/pn-azure.md)] AD) account, you'll automatically be signed in to
[!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)]. If not, use the holographic keyboard to sign in with a work or
school account that has an [!include[pn-office-365](../includes/pn-office-365.md)] Premium or Essentials subscription. Once
you’re signed in, you’ll see your recent contacts.

## Using the user interface or voice commands

The procedures in this user guide describe how to do tasks through the user
interface or by using voice commands, when available. To use a voice command,
say “[!include[pn-remote-assist](../includes/pn-remote-assist.md)],” and then say the voice command. [Learn more about voice
commands.](#voice)

> [!NOTE]
> At this time, voice commands and speech recognition are available only in English for HoloLens 1. For HoloLens 2, voice commands are [available in specific languages](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/faq#what-languages-are-voice-commands-and-speech-recognition-available-for). 

## Make and receive calls

How you make a call depends on whether you're calling a contact in your company or outside your company.

### Make a call to a contact in your company

-   Open the app and [select](https://support.microsoft.com/help/12644) a
    recent contact. If you don’t see the contact you want, select **Search** ![Search](media/e3155cd796106ea0818d8f52c7dbfcbe.png "Search"), and then use the holographic keyboard to enter a name or email address.

When your contact answers the call in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-teams](../includes/pn-teams.md)], they’ll be able to see
what you see in your space—including holograms.

### Make a call to a contact outside your company

You can make or receive a one-to-one call with a Teams user from another company if external access for both companies has been enabled in [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)]. If you're the admin for your organization, to set up external access, see [Set up cross-company calling](cross-company-calling.md).

> [!NOTE]
> At this time, you can't do group calling or file sharing with contacts outside your company. 

To make a call to a contact outside your company:

- Open the app, select  **Search**, and then use the holographic keyboard to enter the full email address of the external user. You *must* enter the full email address. You won't see any search results if you enter just a name or a partial email address.

> [!NOTE] 
> If you're not able to find the contact you're looking for, it might be because external access has not been enabled in [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] for your company or the other company. Contact your administrator for help. 

## Make group calls

You can include up to 50 people in a group call. You can also switch between participants' video feeds and mute participants as needed.

### Invite additional contacts to a call

1. From the call controls, select the **Open Participants** button.

   ![Animation of selecting Open Participants](media/GC_OpenParticipantsList.gif "Animation of selecting Open Participants")

   > [!TIP]
   > Select the **Open Participants** button again if you want to close the pane. 

2. Select one of your recent contacts, or select **Invite Someone** at the bottom of the list. A list of your recent contacts will appear. If the person you'd like to call isn't on the list, enter a name or email address using the holographic keyboard, and then select a name in the search results to start the call. 

   ![Animation of searching for a call](media/GC_SearchCall.gif "Animation of searching for a call")

   > [!TIP]
   > [Learn how to add additional contacts from Microsoft Teams Desktop](https://support.office.com/article/add-someone-to-a-call-in-teams-267fb0c9-275a-4047-8412-7b2654dc29c3). 

### Switch the displayed video feed in a group call 

1. From the call controls, select the **Open Participants** button. 

2. Hover over the participant whose video feed you want to switch to, and then select it. If the participant's video feed is enabled, the video will switch to their feed. 

   > [!TIP] 
   > You can also switch video feeds from the “participant tray” located below the video feed. Hover over the avatar to display the participant's name, and then air tap to switch video feeds. 

### Mute a participant in a group call 

> [!NOTE]
> You can't mute a participant in a one-to-one call.

1. From the call controls, select the **Open Participants** button. 

2. Air tap the mute icon for the participant you want to mute. 

> [!NOTE]
> If you mute a participant, you won't be able to unmute them. They must unmute themselves through [!include[pn-teams](../includes/pn-teams.md)]. 


## Record a call

You can record a call to a file for viewing later. This is a great way to capture a call for training or for record-keeping purposes.

You can record a call in two ways:

- Use the Game bar built into [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PCs.

- Use the [!include[pn-teams](../includes/pn-teams.md)] recording feature.

### Record a call using the Game bar in Windows 10 PCs

1. On a [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 desktop PC, join a call using [!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)].

2. Press **Windows logo key ![Windows logo key](media/windows-logo-key.png "Windows logo key") + G** to open the Game bar.

   ![Game bar](media/game-bar.png "Game bar")

3. Select the **Start Recording** button (or press **Windows logo key ![Windows logo key](media/windows-logo-key.png "Windows logo key") + Alt + R**).

   A small recording menu will appear that shows that the recording is in progress.
   
   ![Recording](media/recording.PNG "Recording")
   
4. To stop recording, select the **Stop Recording** button.

   The video of the recording will appear in your **Videos/Captures** folder.
   
[Learn more about the Game bar.](https://support.xbox.com/xbox-on-windows/social/record-game-clips-game-bar-windows-10)

### Record a call from Teams

[!include[pn-microsoft-teams](../includes/pn-microsoft-teams.md)] supports [cloud-based call recording of group calls](https://support.office.com/article/record-a-meeting-in-teams-34dfbe7f-b07d-4a27-b4c6-de62f1348c24). Recordings are stored and shared through Microsoft Stream.

1.	Start or join the group call.

2.	To start recording, select **More options** (...) > **Start recording**.

    ![Start recording button](media/start-recording.PNG "Start recording button")
 
3.	To stop recording, select **More options** (...) > **Stop recording**.

    ![Stop recording button](media/stop-recording.PNG "Stop recording button") 
 
    The recording is processed (which can take a while) and saved to Microsoft Stream. The person who started the recording receives an email from [!include[pn-microsoft-stream](../includes/pn-microsoft-stream.md)] when the recording is available. It also shows up in the group chat.

## Receive a call from a contact using Microsoft Teams

-   Select **Video** ![Video](media/bae39e2bdb1eafec5c36c76ffa640355.png "Video") (or say “Video”) to accept the call as a video call or **Audio** ![Audio](media/972493ccc469c4ca41c04f96fabf6ba5.png "Audio") (or say “Audio”) to accept it as a voice-only call. To decline the call, select **Ignore** (or say “Ignore”).

> [!NOTE]
> To receive calls when you’re using other apps on [!include[pn-hololens](../includes/pn-hololens.md)], open the
[!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] app. Then use the [bloom gesture](https://support.microsoft.com/help/12644/hololens-use-gestures)
to leave [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)]. Go ahead and use other apps. You’ll get a notification
from [!include[pn-cortana](../includes/pn-cortana.md)] if a [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] call comes in, and you’ll be able to accept or
decline it using your voice.

## Position the call window

You can pin your video feed in your space, or you can have it follow you around.

To pin your video feed:

-   Gaze to position the window, and then select **Pin** ![Pin](media/d213f48b98dc5b8e41318aaa3782c395.png "Pin") (or say “Pin”). To have it follow you again, select **Unpin** ![Unpin](media/1f4f3c48b466bfaa7a222cd4f1158c9c.png "Unpin") (or say “Unpin”).

## Text chat

You can text chat with the other user on the call. The chat window displays just
the text messages sent during the call.

To open the chat window and enter a message:

1.  Select Show ![Show](media/chaticon3.png "Show") (or say “Show”).

2.  Select the text preview field at the bottom of the chat window. This will
    bring up the holographic keyboard.

3.  Do one of the following:

    -   Select characters in the holographic keyboard.

    -   Select **Microphone** ![Microphone](media/microphone3.png "Microphone"), and then dictate your message. [!include[pn-hololens](../includes/pn-hololens.md)] will convert the message into text.

    -   Connect a Bluetooth keyboard directly to the [!include[pn-hololens](../includes/pn-hololens.md)] and type your message.

1.  Select **Send**.

To read previous messages in the chat window:

-   Air tap and drag the chat window.

> [!NOTE]
> If a message is sent from another user when the chat window isn’t
open, you’ll receive a notification.

## Screen-sharing with an expert on Microsoft Teams

When you're working with an expert on a call, the expert can share their desktop or application window with you to assist with the call. When an expert shares their desktop or running application this way, your video feed of the expert will change to a solid color. You'll still be able to use all the tools in the toolbar even though your video feed is no longer displayed.

To move, size, or close the shared window, use the controls at the top right of the shared window.

![Shared-desktop controls](media/screen-sharing-controls.jpg "Shared-desktop controls")

## Collaborate and annotate

Once you’re connected to a video call, your contact will see everything you see
in your space—including your holograms.

Use [HoloLens gestures](https://support.microsoft.com/help/12644) to draw,
place arrows, and add files to your space. Your contact will see your additions,
and will be able to make annotations of their own.

### Add an arrow

1.  Select the **Arrow** tool (or say “Arrow”) during a video call.

2.  Gaze where you want to add the arrow. You'll see a silhouette of the arrow that shows where it will be placed. For example, note the faint arrow in the following screenshot:

    ![Ghost arrow](media/ghost-arrow-before.PNG "Ghost arrow")

3.  Air tap to place the arrow.

    ![Arrow placed](media/ghost-arrow-after.PNG "Arrow placed")

> [!NOTE]
> If you want to specify the direction that the arrow points, air tap and
    hold, and then rotate your hand to position the arrow.

### Draw in your space

1.  Select the **Ink** tool (or say “Ink”) during a video call.

2.  Gaze where you want to draw, and then use tap and hold to draw.

3.  To finish a drawing, raise your finger back up.

### Change arrow or ink color

-   Select **Colors** (or say “Choose colors”), and then choose the one you
    want.

### Add an image or PDF file

Import an image or PDF file from [!include[pn-onedrive-for-business](../includes/pn-onedrive-for-business.md)] and then place it in your
space. For example, add an image of a diagram to assist with the call. The
people you call will be able to see the image or PDF file in the [!include[pn-teams](../includes/pn-teams.md)] app
during a video call.

To add a file:

1.  During a video call, select **[!include[pn-onedrive](../includes/pn-onedrive.md)]** ![OneDrive](media/12b28856b051be23e665c896cd21b7d2.png "OneDrive") (or say “OneDrive”).

2.  Find and select the file you want to add.

To move an image:

1.  Gaze at it, and then select **Move** (or say “Move”).

2.  Tap and hold the image and move your hand to reposition it.

To resize an image:

1.  Gaze at it, and then select **Scale** (or say “Scale”).

2.  Tap and hold a corner of the image, and then move your hand to make it
    bigger or smaller.

To navigate in a PDF file:

| **To**                        | **Do this**                                                                                       |
|-------------------------------|---------------------------------------------------------------------------------------------------|
| Go through pages sequentially | Use the arrow keys                                                                                |
| Jump to a specific page       | Select the page number to bring up the holographic number pad, and then select the page you want. |

### Take a snapshot of your annotations

During a call, you can take a photo of your mixed reality annotations. When you take a photo, a link to the photo is automatically shared through text chat so you can easily refer to it in the call. Or you can save it for work validation or inspection records.

To take a snapshot:

-   Select **Camera** ![Camera](media/cameraicon3.png "Camera") (or say “Camera”), and then air tap (or say “Snap”) to take the photo.

>   The photo is saved to your [!include[pn-hololens](../includes/pn-hololens.md)] camera roll and shared as a link in text chat.

## Make changes

To erase all the arrows and drawings you’ve added during a video call:

-   Select **Erase all** at the top of the call window (or say “Erase all”).

To undo your most recent action, including **Erase all**:

-   Select **Undo** at the top of the call window (or say “Undo”).

## Join a Teams meeting

You can join a Teams meeting directly from Dynamics 365 Remote Assist. This is useful for maintenance and repairs that are scheduled in advance. It's also useful for inspections and other recurring scenarios. 

To join a call:

- Select the **Join Meeting** button below the **Contacts** screen. The **Join Meeting** button appears if the meeting is happening now or sometime in the next 30 minutes.

   ![Join meeting](media/join-meeting.PNG "Join meeting")

## Use voice commands and gaze <a name="voice"></a>

In many cases, you can use voice commands and gaze instead of gestures. Some voice
commands are contextual, so they only work in particular areas of the user
interface. Note that at this time, voice commands and speech recognition are available only in English for HoloLens 1 and in [specific languages for HoloLens 2](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/faq#what-languages-are-voice-commands-and-speech-recognition-available-for). 

> [!IMPORTANT]
> To use a voice command, say “[!include[pn-remote-assist](../includes/pn-remote-assist.md)],” and then say one of the voice commands in the following table. For example, say "[!include[pn-remote-assist](../includes/pn-remote-assist.md)], Move" to enter Move mode for a slate (window). You can also gaze at any button and say “[!include[pn-remote-assist](../includes/pn-remote-assist.md)], Select” to select that button.

| **Voice command**            | **Description**                                                                      |
|------------------------------|--------------------------------------------------------------------------------------|
| **General**                  |                                                                                      |
| Sign out                     | Sign out of [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)].           |
| Up                           | Go up.                                                                               |
| Previous                     | Go to previous page.                                                                 |
| Next                         | Go to next menu.                                                                     |
| Back                         | Go to previous menu.                                                                 |
| Undo                         | Undo the previous action.                                                            |
| **Pin and unpin video feed** |                                                                                      |
| Pin                          | Pin the video feed in your space so it doesn’t follow you around.                    |
| Unpin                        | Unpin the video feed in your space so it follows you around.                         |
| **Call management**          |                                                                                      |
| Call                         | Call a contact.                                                                      |
| Hang up                      | End the call.                                                                        |
| Audio                        | Answer an incoming call with audio only.                                             |
| Video                        | Answer an incoming call with video.                                                  |
| Ignore                       | Decline an incoming call.                                                            |
| Start video                  | Turn on the video for a call.                                                        |
| Stop video                   | Turn off the video in a call.                                                        |
| Mute                         | Mute the call audio.                                                                 |
| Unmute                       | Unmute the call audio.                                                               |
| Search                       | If used in the Contacts window, brings up the Search window to search for a contact. |
| Next                         | If used in the Contacts window, brings up the next contact in the list.              |
| Previous                     | If used in the Contacts window, brings up the previous contact in the list.          |
| Show                         | Show the text chat window.                                                           |
| Hide                         | Hide the text chat window.                                                           |
| **Annotations**              |                                                                                      |
| Arrow                        | Select the **Arrow** tool to place an arrow in your space.                           |
| Ink                          | Select the **Ink** tool to draw on the walls and surfaces of your space.             |
| Move                         | Select the **Move** tool to move an object.                                          |
| Scale                        | Select the **Scale** tool to resize an object.                                       |
| Camera                       | Select the **Camera** tool to take a picture of your space.                          |
| Snap                         | Take a picture when the Camera tool is open.                                         |
| Colors                       | Pick a color.                                                                        |
| Blue                         | Pick the blue color.                                                                 |
| Gray                         | Pick the gray color.                                                                 |
| Green                        | Pick the green color.                                                                |
| Red                          | Pick the red color.                                                                  |
| Yellow                       | Pick the yellow color.                                                               |
| Erase all                    | Remove all visual elements from your space.                                          |
| **Slate (window) management**        |                                                                                      |
| Move                         | Enter Move mode. |
| Select slate                 | After entering Move mode, gaze at the slate you want to move, and then say "Select slate". The slate will start following your gaze.
| Accept                       | After entering Move mode and selecting a slate, place the slate where you are currently gazing by saying "Accept".                                          | 
| Cancel                       | Stops a currently selected slate from following your gaze and returns it to its original position before you started moving it. |
| Scale                        | Enter Scale mode to resize the slate. </br><br>Or, you can gaze to select the Scale tool, and then say "Select" to enter Scale mode.                                                                     |
| Bigger or Smaller            | Make the window bigger or smaller after entering Scale mode. Repeat the "Bigger" or "Smaller" command until the window is the size you want.                          |
| Reset                        | While gazing at a slate that has recently been moved, saying "Reset" will return the slate to its original position.          |
| **[!include[pn-onedrive](../includes/pn-onedrive.md)]**                 |                                                                                      |
| [!include[pn-onedrive](../includes/pn-onedrive.md)]                     | Open [!include[pn-onedrive](../includes/pn-onedrive.md)] at the root folder to insert a file.                                   |
| Close                        | Close [!include[pn-onedrive](../includes/pn-onedrive.md)].                                                                      |
| Next                         | Go to next page in [!include[pn-onedrive](../includes/pn-onedrive.md)].                                                         |
| Previous                     | Go to previous page in [!include[pn-onedrive](../includes/pn-onedrive.md)].                                                     |
| **Other**                    |                                                                                      |
| Settings                     | Go to Settings page.                                                                 |

## Use the Narrator to announce incoming calls

You can turn on the Narrator if you want to take advantage of voice narration for incoming calls. When you turn on incoming call narration, in addition to displaying the incoming caller's name, the caller's name is announced. You can then say "video," "audio," or "ignore" to respond to the incoming call.

To turn on the Narrator for incoming calls:

- Go to Settings, and then select the **On** button for the Narrator.

  ![Open Narrator](media/narrator.PNG "Open Narrator")

## Use Dynamics 365 Remote Assist to get help in another HoloLens app

Having trouble in another [!include[pn-hololens](../includes/pn-hololens.md)] app? Use [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] to show an expert
what’s happening and get some help.

Here’s how:

1.  Open an app on your [!include[pn-hololens](../includes/pn-hololens.md)].

2.  Use the [bloom gesture](https://support.microsoft.com/help/12644/hololens-use-gestures)
    to leave the 3D view, but don’t close the app launcher.

3.  Start [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] and call your contact.

4.  Once the video call is connected, use the bloom gesture to leave [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)]. Your call will remain connected.

5.  Select the live cube of the app you need help with. Once the app has
    launched, your contact will be able to see its content and give you
    guidance.

> [!NOTE]
> When you’re done getting help from your contact, make sure to go back to [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] and disconnect the call. Until you do that, the call will stay connected and your contact will see and hear what’s happening on your [!include[pn-hololens](../includes/pn-hololens.md)].

## Use Dynamics 365 Field Service from Dynamics 365 Remote Assist

If your organization uses [Dynamics 365 Field Service](https://dynamics.microsoft.com/field-service/overview/?&OCID=AID720979_SEM_yeaT05hp&lnkd=Bing_D365_Brand) to manage field service
work orders, you (the first-line worker) can view [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)]
bookings from [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] and call the expert listed in the **Support Contact** field.
This enables you to do heads-up, hands-free calling through [!include[pn-hololens](../includes/pn-hololens.md)] in the
context of a [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] booking.

> [!NOTE]
> For information on setting up and troubleshooting [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] integration if you're an admin, see [Integrate Dyanmics 365 Field Service](troubleshoot-field-service.md). **Note** that [a Dynamics 365 license](https://dynamics.microsoft.com/field-service/overview/?&OCID=AID720979_SEM_yeaT05hp&lnkd=Bing_D365_Brand) is required to view [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] bookings from [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)].

### View a Dynamics 365 Field Service booking and call an expert from Dynamics 365 Remote Assist

1.  In the Contacts menu, select **[!include[pn-dyn-365](../includes/pn-dyn-365.md)]** ![Dynamics 365](media/d365-button3.png "Dynamics 365") to open the **Booking** pane. (Select **[!include[pn-dyn-365](../includes/pn-dyn-365.md)]** ![Dynamics 365](media/d365-button3.png "Dynamics 365") again to close the **Booking** pane.)  
      
    The **Recent Contacts** screen will appear with a **Booking** pane to the
    right.
    
    > [!NOTE]
    > Only bookings with the “In Progress” status are listed.
    
1.  In the **Booking** pane, select the resource (expert). 

    ![Select the resource (expert](media/61c6885a58d179a39e18b3af01554fcc.png "Select the resource (expert)")

1.  In the filtered contacts list, select the tile for the expert. If you don’t
    see the contact you’re looking for, select **Search** to bring up the
    holographic keyboard.  
      
    When you select a contact, you’ll see the following screen. 

    ![Select a contact](media/712a579fd6c37af3087cd31fd01bab74.png "Select a contact")
    
    > [!NOTE]
    > Booking information is blurred out when you’re in a video call, but remains visible during an audio-only call.

### Open a Power BI dashboard from a Dynamics 365 Field Service booking

-   Select a [!include[pn-power-bi](../includes/pn-power-bi.md)] link to open [!include[pn-power-bi](../includes/pn-power-bi.md)] Online in a browser or to open the
    [!include[pn-power-bi](../includes/pn-power-bi.md)] desktop application.
    
    > [!NOTE]
    > When you open a [!include[pn-power-bi](../includes/pn-power-bi.md)] dashboard, [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] closes. If you’re on a call with an expert, the expert will remain on the call. Return to [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] by opening the application again through the applications menu or live cube.

### Modify the default booking view

To modify the default view of information in the **Booking** pane, [edit the view as
you would any Dynamics 365 view](https://docs.microsoft.com/dynamics365/customer-engagement/customize/create-and-edit-views).

### See also
[Set up and use Microsoft Teams with Dynamics 365 Remote Assist](use-microsoft-teams-with-remote-assist.md)<br/>
[How-to videos](videos.md)<br/>
[FAQ](faq.md)<br/>
