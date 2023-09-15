---
title: Make calls in Dynamics 365 Remote Assist on HoloLens 
author: davepinch
description: Make calls with someone inside or outside your organization in Dynamics 365 Remote Assist on HoloLens
ms.author: davepinch
ms.date: 04/13/2022
ms.topic: article
ms.reviewer: v-wendysmith
---

# Make or take calls in Dynamics 365 Remote Assist on HoloLens

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

With Microsoft Dynamics 365 Remote Assist, you can make or take the following types of calls:  

- **One-to-one call**. A one-to-one call includes two participants. For example, if you're repairing a machine and need help on-the-go, you can make a one-to-one call to a remote collaborator who uses Microsoft Teams.

- **Group call**. A group call includes three or more participants. For example, if you're inspecting an asset in a one-to-one call but need a third person's expertise, any participant can add the third person to the call to form a group call.  

- **Meeting**. A meeting is a scheduled call using Teams or Outlook. Meetings can include any number of participants. For example, if you want to have a weekly inspection with your team, you can create a meeting so that everyone receives notifications about the meeting and can join the meeting.

## Supported scenarios

With Dynamics 365 Remote Assist on HoloLens, you can collaborate with:

- A Teams desktop user in a one-to-one call, group call, or meeting scheduled using Microsoft Teams or Outlook. To learn more about different combinations of HoloLens and Teams users on group calls, see [Group calls](#group-calls).

- A Dynamics 365 Remote Assist mobile user in a one-to-one call or group call

- A Teams mobile user in a one-to-one call

> [!NOTE]
> The mixed-reality toolbar will not appear if the Dynamics 365 Remote Assist user joins the call from two different devices.

## Make a one-to-one call to a contact in your company

1. When you open Dynamics 365 Remote Assist, you'll see your recent contacts list in the **Call** tab. To call one of the contacts you see, select the contact. If you don't see the contact you want, select **Search**, and then use the holographic keyboard to enter a name or email address. 

    ![Screenshot of the Dynamics 365 Remote Assist on HoloLens contacts screen.](media/02.00-contacts.png)
    
    > [!NOTE]
    > If your organization has enabled integration with Dynamics 365 Field Service, you can view and call the contact assigned to your Field Service booking. Select the Dynamics 365 Field Service icon (or say, "Remote Assist, Dynamics"), go to your environment and booking, and then select the **Support Contact** listed.
    >
    > ![Screenshot of the Dynamics 365 Remote Assist on HoloLens contacts screen, showing an expanded booking panel.](media/07.01-dynamics-booking.png)
    
2. You may see the following screen that you can use to select an environment to store the call information.

    ![Select environment button highlighted](media/select-environment-2.PNG)
    
    > [!NOTE]
    > You don't have to select an environment to make a call. To start a call without selecting an environment, select **Launch call**. [Learn about storing data for the Calls dashboard](calls-dashboard.md).

3. While you're on a call, you can mute yourself at any point if you need to. You can't mute the other participant in a one-to-one call, however. 

## Make a one-to-one call to a Teams user outside your tenant

You can search, call, and receive a call from a Dynamics 365 Remote Assist user in another tenant if your tenant is federated with that tenant. To call a federated user, open the app, select **Search**, and then use the holographic keyboard to enter their full email address. You won't see any search results if you enter just a name or a partial email address. After you call a federated contact, they will appear in your recent contacts list, so you don't have to search for that contact again.

>[!Note]
> If you can't find the contact you're looking for, it might be because Teams federation ([Teams external access](/microsoftteams/manage-external-access#:~:text=Enable%20your%20Organization%20to%20Communicate%20with%20another%20Teams,your%20organization%2C%20skip%20to%20step%205.%20See%20More.)) has not been enabled. Contact your administrator for help.

## Group calls

A group call can include Dynamics 365 Remote Assist HoloLens users with Dynamics 365 Remote Assist mobile users and Teams desktop users. You can also switch between participants' video feeds and mute participants as needed. [Learn more about joining group calls with Dynamics Remote Assist mobile users and Teams desktop users](./mobile-app/group-calling.md).

You can combine HoloLens users with Teams users in different combinations:

- Multiple HoloLens users can collaborate on the same Dynamics 365 Remote Assist call. 

- Any Teams user can choose any HoloLens user's space to annotate on if there is more than one HoloLens user. 

- Multiple Teams users can annotate on the same HoloLens user's space at the same time.

### Make a group call

1. Start by calling one person, and then select **Open Participants** (![Graphic showing the open participants icon.](media/open-participants.jpg)) or say "Remote Assist, Open Participants."

    You'll see the first person you called on the left side of the video card, and a list of participants on the right side. 

2. On the bottom of the video card, select the text field to pop out a holographic keyboard with a list of your recent contacts. If the person you want to call isn't on the list, enter a name or email address using the holographic keyboard, and then select a name in the search results to start the call.

To mute a participant in a group call:

1. Select **Open Participants** (![Graphic showing the open participants icon.](media/open-participants.jpg)) or say "Remote Assist, Open Participants." 

2. Tap a participant to see their video feed. 

3. Tap the mute button next to the participant's name to mute them. Muted participants can unmute themselves. Other people on the call can't unmute a muted participant.

> [!Note]
> If the call includes a large number of participants, you might experience performance issues, such as delays in viewing annotations and lower video resolution. [Learn more about the number of participants that can join a Microsoft Teams call](/microsoftteams/limits-specifications-teams#meetings-and-calls). 

## Accept a call

You can do any of the following when you receive a call:

- Select **Video** (or say "Remote Assist, Video") to accept the call as a video call.

- Select **Audio** (or say "Remote Assist, Audio") to accept the call as a voice-only call. 

- Select **Ignore** (or say "Remote Assist, Ignore") to decline the call.

If you join the call, remote collaborators will be able to see what you see in your space, including holograms.

> [!Note]
> In you're using another HoloLens app, you can have Dynamics 365 Remote Assist run in the background to receive any incoming calls. To do this, first open Dynamics 365 Remote Assist. Then use the Start gesture to go to the **Start** menu and select another app to use. You'll get a notification if a Dynamics 365 Remote Assist call comes in, and you'll be able to select **Accept** to initiate an audio call, **Video** to initiate a video call, or **Ignore** to ignore the call.

## End a call

- Select **End Call** (![Graphic showing the end call icon.](media/end-call.jpg)), or say "Remote Assist, End Call."

## Adjusting outgoing video quality if the HoloLens device gets too hot

If you're on a longer call in Dynamics 365 Remote Assist for HoloLens, the HoloLens device can become hot if it's using several device capabilities at the same time (for example, multiple cameras, Mixed Reality Capture, and wi-fi). To extend the length of the call and keep the device from overheating, Dynamics 365 Remote Assist gradually reduces outgoing video quality. If this happens, you'll see a series of messages to let you know how and why the outgoing video quality is being adjusted. [Learn more about how Dynamics 365 Remote Assist adjusts video quality](hololens-thermal-adjusting.md)

### Learn more 
- [Group calls between Dynamics 365 Remote Assist mobile, Dynamics 365 Remote Assist HoloLens, and Teams desktop](./mobile-app/group-calling.md).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
