---
title: Call a remote collaborator on Microsoft Teams from Dynamics 365 Guides  
author: 
description: 
ms.author: 
ms.date: 11/12/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Call a remote collaborator on Microsoft Teams from Dynamics 365 Guides 

When you're working in Microsoft Dynamics 365 Guides on HoloLens, if you need help with a task in your world, you might want to call a remote collaborator on Microsoft Teams (desktop or mobile) or Dynamics 365 Remote Assist. 

Dynamics 365 Guides supports the following types of calls:  

- **One-to-one call**. A one-to-one call includes two participants. For example, if you need help with a machine that you're repairing, start a one-to-one call with a remote expert.

- **Group call**. A group call includes three or more participants. For example, if you're inspecting an asset in a one-to-one call but need a third person's expertise, any call participant can add the third person to form a group call. 
    
- **Meeting**. A meeting is a call scheduled through Teams or Outlook. Meetings can include any number of participants. For example, if you want to have a weekly inspection with your team, create a meeting so that everyone receives notifications about the meeting and can join the meeting. [Learn how to join a meeting from Dynamics 365 Guides](calling-meetings.md)

> [!NOTE]
> An adminstrator can remove the ability for a user to see video in a call. In this case, the user joins the call with audio only. [Learn more about Teams policies supported by Dynamics 365 Guides](admin-teams-policies.md)

## Who can collaborate on a call?

A Dynamics 365 Guides HoloLens user can collaborate with:

- A Teams desktop user (PC or Mac) on a one-to-one call, group call, or scheduled meeting. To learn more about different combinations of HoloLens and Teams users on group calls, see [Group calls](#group-calls).

- A Dynamics 365 Remote Assist mobile user on a one-to-one or group call.

- A Teams mobile user on a one-to-one call.

> [!NOTE]
> The mixed-reality toolbar will not appear if the Dynamics 365 Guides user joins the call from two different devices.

## Start a call from Dynamics 365 Guides

> [!NOTE]
> At this time, you can't receive a call in Dynamics 365 Guides from a Teams or Dynamics 365 Remote Assist user. You must initiate the call from Dynamics 365 Guides. 

### Start a one-to-one call with a Teams contact in your organization 

1. Look at the palm of your hand to open the Main menu, and then select the **Communications** button.

    ![Screenshot of Communications button on Main menu.](media/calling-meetings-1.JPG "Screenshot of Communications button on Main menu")    
        
2. Do one of the following:

    - If the contact you want to call is listed in the **Recent** list, select the contact.      

    - If the contact isn't listed in the **Recent** list, place your cursor in the **Search** box, and then in the holographic keyboard that appears, enter the person's name or email address. Use the **Microphone** button if you prefer to use your voice to enter the person's name in the **Search** box. 

      ![Screenshot of Recent list with Search box below and holographic keyboard displayed.](media/calling-start-call-1.JPG "Screenshot of Recent list with Search box below and holographic keyboard displayed")   
    
3. In the window that appears, select the **Phone** button to call the contact. 

      ![Screenshot of call details screen.](media/calling-start-call-2.JPG "Screenshot of call details screen")

    You'll see the contact's video feed, activity controls, calling controls, and the **Annotate** toolbar. The green indicator below the activity controls shows that you're on a call with that contact. This is useful as a reminder in case you select a different type of activity, such as opening a guide or file. 

    ![Screenshot of video feed, controls, and Annotate toolbar.](media/calling-start-call-3.JPG "Screenshot of video feed, controls, and Annotate toolbar")
    
> [!NOTE]
> You can't mute or remove a call participant in a one-to-one call. 
       
### Start a one-to-one call with a Teams contact outside your organization

You can search for and call a Teams contact in another organization if your organization is federated with that organization. To call a federated contact, open Dynamics 365 Guides, select **Search**, and then use the holographic keyboard to enter their **full email address** (or use the **Microphone** button if you prefer to use your voice). You won't see any search results if you enter just a name or a partial email address. 

After you call a federated contact, they appear in your recent contacts list, so you don't have to search for that contact again.

>[!Note]
> If you can't find the contact you're looking for, it might be because Teams federation ([Teams external access](/microsoftteams/manage-external-access#:~:text=Enable%20your%20Organization%20to%20Communicate%20with%20another%20Teams,your%20organization%2C%20skip%20to%20step%205.%20See%20More.)) has not been enabled. Contact your administrator for help.

### Group calls

A group call can include a Dynamics 365 Guides user on HoloLens and a Teams desktop user (PC or Mac) or Dynamics 365 Remote Assist mobile user. 

> [!NOTE]
> A Teams mobile user cannot collaborate on a group call with a Dynamics 365 Guides user on HoloLens.

On group calls, you can switch between participants' video feeds and mute or remove participants as needed. 

You can combine HoloLens users with Teams users in different combinations:

- Multiple HoloLens users can collaborate on the same Dynamics 365 Guides call. 

- Any Teams desktop user can choose any HoloLens user's space to annotate on if there is more than one HoloLens user. 

- Multiple Teams desktop users can annotate on the same HoloLens user's space at the same time.

#### Start a group call 

1. Start by calling one person as described above for a one-to-one call, and then select the **Open Participants** button (or say "Guides, Open Participants"). When you select the **Open Participants** button, tiles for all participants on the call appear to the right of the video feed. The first tile shows the first person that you called. 

    ![Screenshot of one-to-one call with Open Participants button highlighted.](media/calling-start-call-4.JPG "Screenshot of one-to-one call with Open Participants button highlighted")
        
2. Select the **Participants** button in the Participants area (to the right of the video feed) to display a list of recent contacts.

    ![Screenshot of right side of screen with Participants button highlighted.](media/calling-start-call-5.JPG "Screenshot of right side of screen with Participants button highlighted")
   
3. Do one of the following:

    - If the contact you want to add is listed in the **Recent** list, select the contact's tile, and then select **Show video**.

    - If the contact isn't listed in the **Recent** list, place your cursor in the **Search** box, and then in the holographic keyboard that appears, enter the person's name or email address. Use the **Microphone** button if you prefer to use your voice to enter the person's name in the **Search** box. 

      ![Screenshot of Recent list with Search box and holographic keyboard showing.](media/calling-start-call-6.JPG "Screenshot of Recent list with Search box and holographic keyboard showing")
      
#### Mute a participant in a group call

1. Select the **Open Participants** button or say "Guides, Open Participants." 

2. Select the tile for the participant that you want to mute.

3. When the tile flips over, select **Mute**. Muted participants can unmute themselves. 

> [!Note]
> If the call includes a large number of participants, you might experience performance issues, such as delays in viewing annotations and lower video resolution. [Learn more about the number of participants that can join a Microsoft Teams call](/microsoftteams/limits-specifications-teams#meetings-and-calls). 

#### Remove a participant in a group call

1. Select the **Open Participants** button or say "Guides, Open Participants." 

2. Select the tile for the participant that you want to remove.

3. When the tile flips over, select **Remove**.

#### Spotlighting in Dynamics 365 Guides 

Dynamics 365 Guides supports [Teams spotlighting](https://support.microsoft.com/en-us/office/spotlight-someone-s-video-in-a-teams-meeting-58be74a4-efac-4e89-a212-8d198182081e). When someone is spotlighted in Teams, the video feed in Dynamics 365 Guides changes to show the spotlighted person. If the spotlighted person is the Dynamics 365 Guides user, the user will see a notification above the video feed that indicates that they've been spotlighted.

A Dynamics 365 Guides user cannot spotlight anyone else on the call, including themselves.  

### End a call

- Select the **End call** button or say "Guides, End call."

### How outgoing video quality is adjusted if the HoloLens device gets too hot

If you're on a longer call, the HoloLens device can become hot if it's using several device capabilities at the same time (for example, multiple cameras, Mixed Reality Capture, and Wi-Fi). To extend the length of the call and keep the device from overheating, Dynamics 365 Guides gradually reduces outgoing video quality. If this happens, you'll see a series of messages to let you know how and why the outgoing video quality is being adjusted. [Learn more about how Dynamics 365 Guides automatically adjusts video quality](calling-hololens-thermal-adjusting.md)

## Receive a call in Teams desktop (PC or Mac) from a Dynamics 365 Guides user 

> [!NOTE]
> At this time, you can't call a Dynamics 365 Guides user from Teams desktop. The Dynamics 365 Guides user must initiate the call. 

1. Launch the Teams app.

   > [!IMPORTANT]
   > If this is the first time you have launched Teams and you have not been invited to any other teams, Teams will automatically take you to the correct place. If you have been invited to other teams, you might need to switch to the appropriate organization.  
   >     
   > To switch organizations, in the drop-down menu in the upper-right corner of the window, select the appropriate guest organization. Teams might take a few seconds to reload.

 2. When you see an incoming call notification at the bottom right side of your screen, select **Audio** or **Video** to join the call.

### Use the call controls

When you're on a call, you'll see the call controls at the bottom of the screen. The following table describes the call controls. 

|Button|Description|
|------------|----------------------------------------------|
|![Video button.](media/calling-teams-video-button.JPG)|Control outgoing video.|
|![Microphone button.](media/calling-teams-audio-button.JPG)|Control outgoing audio.|
|![Share button.](media/calling-teams-share-button.JPG)|Share your desktop or a running application.|
|![Chat button.](media/calling-teams-chat-button.JPG)|Open a chat window to send text messages.| 
|![Participants button.](media/calling-teams-participants-button.JPG)|See current participants, or add more.|

To use additional features, select the **More info** […] button. For example, select **Blur my background** if you have sensitive information behind you or want to protect the privacy of colleagues who are behind you. If you want to record the meeting, you can access the **Record** command here. 

## Receive a call in Teams mobile from a Dynamics 365 Guides user 

> [!NOTE]
> At this time, you can't call a Dynamics 365 Guides user from Teams mobile. The Dynamics 365 Guides user must initiate the call. 

Use the call controls at the bottom of the screen in Teams mobile for the following actions.

|Button|Description|
|------------|----------------------------------------------|
|![Video button.](media/calling-teams-mobile-video-button.JPG)|Control outgoing video.|
|![Microphone button.](media/calling-teams-mobile-audio-button.JPG)|Control outgoing audio.|
|![Speaker button.](media/calling-teams-mobile-speaker-button.JPG)|Control incoming audio.|

Select the **More info** [...] button to access the following additional commands:

- **Toggle incoming video**: Turn incoming video off or on. You might want to do this to conserve your battery on your device or if incoming video is distracting. 
- **Share your screen**: Your screen will pop up as a video for the Dynamics 365 Guides user.
- **Start video with blur**: For iOS devices only, if you have sensitive information behind you or want to protect the privacy of colleagues who are behind you, select this command. 
- **Insert file**: Share a file.  

> [!TIP]
> Turn your phone horizonal to see more of the Dynamics 365 Guides user’s environment.  

## See also

- [Join a scheduled meeting](calling-meetings.md)
- [Chat](calling-chat-file-sharing.md)
- [Record a call](calling-record-call.md)
- [Screen and file sharing](calling-screen-sharing.md)
- [Annotations](calling-annotations.md)
- [Access OneDrive files](onedrive-files.md)
- [Teams users capabilities](calling-teams-users.md)
- [Where call data is stored](call-logging.md)

