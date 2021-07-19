---
title: Make calls in Dynamics 365 Remote Assist on HoloLens 
author: sophiasysun
description: Make calls with someone inside or outside your organization in Dynamics 365 Remote Assist on HoloLens
ms.author: sopsun
ms.date: 07/19/2021
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Make or take calls in Dynamics 365 Remote Assist on HoloLens

With Microsoft Dynamics 365 Remote Assist, you can make or take the following types of calls:  

- **One-to-one call**. A one-to-one call includes two participants. For example, if you're repairing a machine and need help on-the-go, you can make a one-to-one call to a remote collaborator who uses Microsoft Teams.

- **Group call**. A group call includes three or more participants. For example, if you're inspecting an asset in a one-to-one call but need a third person's expertise, any participant can add the third person to the call to form a group call.  

- **Meeting**. A meeting is a scheduled call using Teams or Outlook. Meetings can include any number of participants. For example, if you want to have a weekly inspection with your team, you can create a meeting so that everyone receives notifications about the meeting and can join the meeting.

## Supported scenarios

With Dynamics 365 Remote Assist on HoloLens, you can collaborate with:

- A Teams desktop user in a one-to-one call, group call, or meeting scheduled using Microsoft Teams or Outlook

- A Dynamics 365 Remote Assist mobile user in a one-to-one call or group call

- A Teams mobile user in a one-to-one call

> [!NOTE]
> The mixed-reality toolbar will not appear if the Dynamics 365 Remote Assist user joins the call from two different devices.

## Make a one-to-one call to a contact in your company

1. When you open Dynamics 365 Remote Assist, you'll see your recent contacts list in the **Call** tab. To call one of the contacts you see, select the contact. If you don't see the contact you want, select **Search**, and then use the holographic keyboard to enter a name or email address. 

    ![Screenshot of the Dynamics 365 Remote Assist on HoloLens contacts screen.](media/02.00-contacts.png)
    
    > [!NOTE]
    > If your organization has enabled integration with Dynamics 365 Field Service, you can view and call the contact assigned to your Field Service booking. Select the Dynamics 365 Field Service icon (or say, "Remote Assist, Dynamics"), go to your instance and booking, and then select the **Support Contact** listed.
    >
    > ![Screenshot of the Dynamics 365 Remote Assist on HoloLens contacts screen, showing an expanded booking panel.](media/07.01-dynamics-booking.png)
    
2. Select the environment where you want to store the call information.

    ![Select environment button highlighted](media/select-environment-2.PNG)
    
    > [!NOTE]
    > You don't have to select an environment to make a call. To start a call without selecting an environment, select **Launch call**. [Learn about storing data for the Calls dashboard](calls-dashboard.md).

3. While you're on a call, you can mute yourself at any point if you need to. You can't mute the other participant in a one-to-one call, however. 

## Make a one-to-one call to a Teams user outside your tenant

You can search, call, and receive a call from a Dynamics 365 Remote Assist user in another tenant if your tenant is federated with that tenant. To call a federated user, open the app, select **Search**, and then use the holographic keyboard to enter their full email address. You won't see any search results if you enter just a name or a partial email address. After you call a federated contact, they will appear in your recent contacts list, so you don't have to search for that contact again.

>[!Note]
> If you can't find the contact you're looking for, it might be because Teams federation ([Teams external access](/microsoftteams/manage-external-access) has not been enabled. Contact your administrator for help.

## Make a group call

A group call can include Dynamics 365 Remote Assist HoloLens or HoloLens 2 users with Dynamics 365 Remote Assist mobile users and Teams desktop users. You can also switch between participants' video feeds and mute participants as needed. [Learn more about joining group calls with Dynamics Remote Assist mobile users and Teams desktop users](./mobile-app/group-calling.md).

Start by calling one person, and then select **Open Participants** (![Graphic showing the open participants icon.](media/RAHL_Participants.png)).

You'll see the first person you called on the left side of the video card, and a list of participants on the right side. On the bottom of the video card, select the text field, to pop out a holographic keyboard with a list of your recent contacts. If the person you want to call isn't on the list, enter a name or email address using the holographic keyboard, and then select a name in the search results to start the call.

To mute a participant:

1. Select **Open Participants** or say "Remote Assist, Open Participants." 

2. Tap a participant to see their video feed. 

3. Tap the mute button next to a participant's name to mute them. Muted participants can unmute themselves.

> [!Note]
> If the call includes a large number of participants, you might experience performance issues, such as delays in viewing annotations and lower video resolution. [Learn more about the number of participants that can join a Microsoft Teams call](/MicrosoftTeams/limits-specifications-teams#meetings-and-calls). 

## Accept a call

Select **Video** (or say "Remote Assist, Video") to accept the call as a video call or **Audio** (or say "Remote Assist, Audio") to accept it as a voice-only call. To decline the call, select **Ignore** (or say "Remote Assist, Ignore").

> [!Note]
> To receive calls when you're using other apps on HoloLens, first open the Dynamics 365 Remote Assist app. Then use the **Start** gesture to go to the start menu, and select another app to use. This keeps Dynamics 365 Remote Assist running in the background.
>
> You'll get a notification if a Dynamics 365 Remote Assist call comes in, and you'll be able to select **Accept** to initiate an audio call, **Video** to initiate a video call, and **Ignore** to ignore the call.
>
> In other words, you can receive a call in two scenarios – if Dynamics 365 Remote Assist is the app you have open and if it's running in the background.

When you join the call, remote collaborators will be able to see what you see in your space—including holograms.

## End a call

To end a call, select **End Call** (as seen here: ![Graphic showing the end call icon.](media/RAHL_EndCall.png)), or say "Remote Assist, End Call."

### Learn more 
- View documentation on group calls between Dynamics 365 Remote Assist mobile, Dynamics 365 Remote Assist HoloLens, and Teams desktop [here](./mobile-app/group-calling.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
