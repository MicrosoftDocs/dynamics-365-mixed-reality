---
title: One-to-one and group calls in Dynamics 365 Guides on HoloLens 
author: 
description: 
ms.author: 
ms.date: 11/14/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Start a call in Dynamics 365 Guides on HoloLens 

With Microsoft Dynamics 365 Guides, you can have the following types of calls:  

- **One-to-one call**. A one-to-one call includes two participants. For example, if you're repairing a machine and need help on-the-go, you can start a one-to-one call with a remote collaborator on Microsoft Teams or Dynamics 365 Remote Assist.

- **Group call**. A group call includes three or more participants. For example, if you're inspecting an asset in a one-to-one call but need a third person's expertise, any participant can add the third person to the call to form a group call. 
    
- **Meeting**. A meeting is a scheduled call using Teams or Outlook. Meetings can include any number of participants. For example, if you want to have a weekly inspection with your team, you can create a meeting so that everyone receives notifications about the meeting and can join the meeting. [Learn more about joining a meeting in Dynamics 365 Guides](calling-meetings.md)

## Who can you collaborate with on a call?

With Dynamics 365 Guides on HoloLens, you can collaborate with:

- A Teams desktop user (PC or Mac) on a one-to-one call, group call, or scheduled meeting that's set up through Teams or Outlook. To learn more about different combinations of HoloLens and Teams users on group calls, see [Group calls](#group-calls).

- A Teams mobile user on a one-to-one call.

- A Dynamics 365 Remote Assist mobile user on a one-to-one or group call.

> [!NOTE]
> The mixed-reality toolbar will not appear if the Dynamics 365 Guides user joins the call from two different devices.

## Start or receive a call in Dynamics 365 Guides

### Make a one-to-one call to a contact in your organization 

1. Look at the palm of your hand to open the Main menu, and then select the **Communications** button.

    ![Screenshot of Communications button on Main menu.](media/calling-meetings-1.JPG "Screenshot of Communications button on Main menu")    
        
2. Select the contact that you want to call.

    ![XXX.](media/calling-start-call-1.JPG "XXX")
    
3. In the Call window that appears, select the **Phone** button. 

    ![XXX.](media/calling-start-call-2.JPG "XXX")

   You'll see the contact's video feed. The green indicator to the lower left of the video feed shows that you're on a call with that contact. This is useful if you select a different activity such as opening a guide or file. 

    ![XXX.](media/calling-start-call-3.JPG "XXX")
    
### Make a one-to-one call to a Teams user outside your organization

You can search, call, and receive a call from a Teams user in another organization if your organization is federated with that tenant. To call a federated user, open Dynamics 365 Guides, select **Search**, and then use the holographic keyboard to enter their **full email address** (or use the **Mic** button if you prefer to use your voice). You won't see any search results if you enter just a name or a partial email address. 

After you call a federated contact, they will appear in your recent contacts list, so you don't have to search for that contact again.

>[!Note]
> If you can't find the contact you're looking for, it might be because Teams federation ([Teams external access](/microsoftteams/manage-external-access#:~:text=Enable%20your%20Organization%20to%20Communicate%20with%20another%20Teams,your%20organization%2C%20skip%20to%20step%205.%20See%20More.)) has not been enabled. Contact your administrator for help.

### Group calls in Dynamics 365 Guides 

A group call can include a Dynamics 365 Guides user on HoloLens and a Teams desktop user (PC or Mac) or Dynamics 365 Remote Assist mobile user. 

> [!NOTE]
> A Teams mobile user cannot collaborate on a group call with a Dynamics 365 Guides user on HoloLens.

On grooup calls, you can switch between participants' video feeds and mute or remove participants as needed. 

You can combine HoloLens users with Teams users in different combinations:

- Multiple HoloLens users can collaborate on the same Dynamics 365 Guides call. 

- Any Teams desktop user can choose any HoloLens user's space to annotate on if there is more than one HoloLens user. 

- Multiple Teams desktop users can annotate on the same HoloLens user's space at the same time.

#### Start a group call 

1. Start by calling one person as described above, and then select the **Open Participants** button (or say "Guides, Open Participants).

    ![XXX.](media/calling-start-call-4.JPG "XXX")

    You'll see the tile for the first person you called on the right side of the video feed. 
    
2. Select the **Participants** button in the Participants area to display a list of recent contacts.

    ![XXX.](media/calling-start-call- .JPG "XXX")
   
3. Do one of the following:

    - If the person you want to add is listed in the **Recent** list, select the contact's tile, and then select **Show video**.

      ![XXX.](media/calling-start-call- .JPG "XXX")
 
    - If the person isn't listed in the **Recent** list, place your cursor in the Search box, to display the holographic keyboard, and then use the holographic keyboard to enter the person's name or email address. You can also use the **Mic** button if you prefer to use your voice to enter the person's name in the Search box. 

      ![XXX.](media/calling-start-call- .JPG "XXX")
      
#### Mute a participant in a group call

1. Select the **Open Participants** button or say "Guides, Open Participants." 

2. Select the tile for the participant that you want to mute.

3. When the tile flips over, select **Mute**

    ![XXX.](media/calling-start-call- .JPG "XXX")


    > [!NOTE]
    > Muted participants can unmute themselves. Other people on the call can't unmute a muted participant.

> [!Note]
> If the call includes a large number of participants, you might experience performance issues, such as delays in viewing annotations and lower video resolution. [Learn more about the number of participants that can join a Microsoft Teams call](/microsoftteams/limits-specifications-teams#meetings-and-calls). 

#### Remove a participant in a group call

1. Select the **Open Participants** button or say "Guides, Open Participants." 

2. Select the tile for the participant that you want to remove.

3. When the tile flips over, select **Remove**

    ![XXX.](media/calling-start-call- .JPG "XXX")

### Accept a call

At this time, you can't accept a call from a Teams or Dynamics 365 Remote Assist user in Dynamics 365 Guides. You must initiate the call from Dynamics 365 Guides. 

### End a call

- Select the **End Call** button or say "Guides, End Call."

   ![XXX.](media/calling-start-call- .JPG "XXX")

### Adjust outgoing video quality if the HoloLens device gets too hot

If you're on a longer call in Dynamics 365 Guides on HoloLens, the HoloLens device can become hot if it's using several device capabilities at the same time (for example, multiple cameras, Mixed Reality Capture, and Wi-Fi). To extend the length of the call and keep the device from overheating, Dynamics 365 Guides gradually reduces outgoing video quality. If this happens, you'll see a series of messages to let you know how and why the outgoing video quality is being adjusted. [Learn more about how Dynamics 365 Guides adjusts video quality](calling-hololens-thermal-adjusting.md)
