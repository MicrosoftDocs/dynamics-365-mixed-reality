---
title: Record calls in Dynamics 365 Remote Assist on HoloLens 
description: Use cloud-based recording or several other alternatives in Microsoft Dynamics 365 Remote Assist on HoloLens
author:  BogdanBerg
ms.author: bogdanb
ms.date: 07/08/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
---

# Record calls in Dynamics 365 Remote Assist on HoloLens

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

Recording a call is great for training or record-keeping purposes. Cloud-based recordings are automatically uploaded to Microsoft OneDrive or SharePoint. When the recording finishes uploading, all call participants can access the link in the Teams chat.

Read about the [layout](#cloud-based-recording-layout) of this type of call before deciding whether to record using this method. You might also consider [alternatives to cloud-based recordings](#alternatives-to-cloud-based-recording).

## Overview of cloud-based recording

Remote Assist HoloLens users, Teams desktop, and Teams mobile users can initiate one-to-one and group calls and meetings.

Exceptions include:

- An unlicensed one-time call participant.

- Call participant without the [required license](/microsoftteams/cloud-recording#prerequisites-for-teams-cloud-meeting-recording).

- Other exceptions described by [Microsoft Teams documentation](/microsoftteams/cloud-recording#prerequisites-for-teams-cloud-meeting-recording).

Learn more about using [Teams desktop](https://support.office.com/article/Record-a-meeting-in-Teams-34dfbe7f-b07d-4a27-b4c6-de62f1348c24) to record the call.

> [!Note]
> The recorder is the owner of the video. The owner needs to [give permission](https://support.office.com/article/Play-and-share-a-meeting-recording-in-Teams-7d7e5dc5-9ae4-4b94-8589-27496037e8fa#bkmk_sharemeetingrecording) or [download](https://support.office.com/article/Play-and-share-a-meeting-recording-in-Teams-7d7e5dc5-9ae4-4b94-8589-27496037e8fa#bkmk_downloadmeetingrecording) the video to share the recording beyond people on the call.  

## Use cloud-based recording

1. Select the **Recording** button (![Start recording button.](media/RAHL_CallRecording_StartButton.png)).

    ![Screenshot of Dynamics 365 Remote Assist on HoloLens, showing the record button.](media/03.00-call.png)

   A reminder that the call recording only captures the middle vertical section of your field of view appears. If there are procedures or assets that are critical for you to record, keep them in the middle of your field of view. Learn more about [Teams recording layout for calls with two participants](#cloud-based-recording-layout).

1. Select **OK** to start recording. An indicator lets you know that you're recording. This indicator remains visible even if you do another action such as opening a file.

1. To end the recording, press the **Recording** (![Stop recording button.](media/RAHL_CallRecording_StopButton.png)) button or end the call. A reminder indicates that the recording is being processed and saved securely in OneDrive for work or SharePoint.  

After the recording is processed and saved, it appears in your Dynamics 365 Remote Assist chat history (if you're still in the call) and also your Teams chat history. Remember that your Dynamics 365 Remote Assist chat history doesn't persist when the call ends, but your Teams chat history does. To view the recording in your HoloLens browser, select the link in the Dynamics 365 Remote Assist chat.

## Cloud-based recording layout

The layout of the cloud-based recording depends on the number of call participants, and the layout can't be configured. When using Dynamics 365 Remote Assist or Teams to record the call, the Dynamics 365 Remote Assist HoloLens user's view (their outgoing video feed) never occupies the entire recording unless the HoloLens user is the only person in a call or meeting.

If the [explicit recording consent for Teams Audio Conferencing](/microsoftteams/conferencing-recording-consent) is enabled and you record a call, some unexpected behavior might occur such as users can't unmute themselves.

If it's imperative that your recording captures as much of the Dynamics 365 Remote Assist HoloLens user's view as possible and as little of the Teams user's outgoing video feed or avatars, consider using [one of the alternative recording methods](#alternatives-to-cloud-based-recording).

Review several examples of what the recording layout looks like when you use Teams or Dynamics 365 Remote Assist to record.

- In a recording with two participants, each participant's outgoing video (or avatar) occupies one-half of the recording. Both halves are vertical. During a Dynamics 365 Remote Assist call, a Teams desktop user sees a horizontal slice of what you see. But the recording only captures the middle vertical slice of what you see. Furthermore, during the Dynamics 365 Remote Assist call, the Teams user only sees their outgoing video feed in the corner of the call, but in the recording, their outgoing video feed occupies half the recording. (If the Teams user turns off their outgoing video feed, their avatar occupies half the recording.)

    ![Screenshot of Teams recording, showing half the screen with the HoloLens participant, and the other half with the Teams avatar.](media/2call.png)

- In a recording with three participants, each participant's outgoing video (or avatar) occupies one-third of the recording. Furthermore, during the Dynamics 365 Remote Assist call, the Teams user only sees their outgoing video feed in the corner of the call, but in the recording, their outgoing video feed occupies one third the recording. (If the Teams user turns off their outgoing video feed, their avatar occupies one third of the recording.)

    ![Screenshot of Teams recording, showing three participants.](media/3call.png)

- In a recording with four participants, each participant's outgoing video (or avatar) occupies one-fourth of the recording. During the Dynamics 365 Remote Assist call, the Teams user only sees their outgoing video feed in the corner of the call, but in the recording, their outgoing video feed occupies one fourth of the recording. (If the Teams user turns off their outgoing video feed, their avatar occupies one fourth of the recording.)  

    ![Screenshot of Teams recording, showing four participants.](media/4call.png)

- In a recording with five or more participants, the horizontal recording splits into four, with remaining participants' avatars in the bottom-right corner of the recording.

    ![Screenshot of Teams recording, showing the same four participants, with an additional participant avatar at the bottom right.](media/5call.png)

## Alternatives to cloud-based recording

### Use the HoloLens operating system

Use this option when:

- No call participant can initiate a cloud-based call recording.

- You only want the recording to capture what you see through the HoloLens, what you hear around you, and what you hear through the HoloLens speakers. For example, the recording only shows the participants in the Dynamics 365 Remote Assist call if you manually navigate to the participants panel and it is in your field of view.

There are three ways to use the HoloLens operating system.

#### Use the HoloLens app

1. From the **Start** menu, select the **Video** button from the bottom tool pane.
  
1. Air tap when you're ready to record.
  
1. To stop recording, perform the **Start Gesture**, and then press the **Video** button again.
  
   ![Screenshot from the HoloLens field of view, showing the video icon on the bottom tool pane.](media/RAHL_OSVideo.png)

    > [!NOTE]
    > If you use this method to record your environment outside a call, joining a call will end the recording.

#### Use your voice

1. Say "Record call." A short countdown occurs, and then the recording starts. A red recording indicator in the top right-hand corner of your view indicates the recording is live.

1. To stop recording, say "Stop recording." The video is saved to your **Camera Roll**. Use the **Start** menu to go to your camera roll.

#### Use the HoloLens hardware

1. Press and hold the volume-up and volume-down buttons simultaneously until a three-second countdown begins.

1. To stop recording, tap both buttons simultaneously. The video is saved to the HoloLens camera roll. The video doesn't upload automatically.

1. To get a photo or video off the HoloLens camera roll, choose one of the following methods:

   - Upload to OneDrive: Sign into OneDrive and upload your file.

   - Connect to a PC with a USB-C cable: On a PC, access the internal storage through File Explorer. Go to **Pictures** > **Camera Roll folder** and copy your images or videos from this folder.

    [Learn more about taking photos and videos and getting them off the device](/hololens/holographic-photos-and-videos#capture-a-mixed-reality-photo).

### Ask a Teams desktop user to use the Windows Game Bar

Use this option when you want the recording to capture exactly what the Teams desktop user sees during the call. For example, you want to see the Teams user interface and call layout the Teams desktop user configures.

Go to [How a Teams desktop user can record a call using Windows Game Bar](teams-pc-all.md#record-your-teams-desktop-screen-using-windows-game-bar). Learn more about the [Windows Game Bar](https://support.xbox.com/help/friends-social-activity/share-socialize/record-game-clips-game-bar-windows-10).

[!INCLUDE[footer-include](../includes/footer-banner.md)]
