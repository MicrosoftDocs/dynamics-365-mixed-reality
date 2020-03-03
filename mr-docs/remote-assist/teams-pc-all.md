---
author: sopsun
description: Collaborate with a Remote Assist user via Microsoft Teams on PC
ms.author: sopsun
ms.date: 02/17/2020
ms.service: crm-online
ms.topic: article
title: Collaborate with a Remote Assist user via Microsoft Teams on PC
ms.reviewer: krbjoran
---
# Collaborate with a Remote Assist user via Microsoft Teams on PC

## Overview

When you use Teams on a PC running Windows 10, you can collaborate with people using Remote Assist on HoloLens 1 or 2 (a “Remote Assist HoloLens user”) or Remote Assist on a mobile device (a “Remote Assist mobile user”).   
However, the features you can use to collaborate differ depending on which platform the Remote Assist user is using.  

### Feature comparison: Collaborating with Remote Assist HoloLens user versus Remote Assist mobile user

### Key terms

When you join a call, you will see the mixed reality toolbar.   
![MRT](media/PC_MRToolbar.png "MRT")


And the call controls panel. 
![PC_CallControls](media/PC_CallControls.png "PC_CallControls")
 
The More Options panel ![MoreOptions](media/PC_MoreOptions.png "MoreOptions")includes additional features. 


## Launch Teams 

Launch the Teams app.

    > [!IMPORTANT]
    > If this is the first time the expert has launched [!include[pn-teams](../includes/pn-teams.md)] and the expert has not been invited to any other teams, [!include[pn-teams](../includes/pn-teams.md)] will automatically take the expert to the correct place. If the expert has been invited to other teams, the expert might need to switch to the appropriate tenant.  
    >     
    > To switch tenants, in the drop-down menu in the upper-right corner of the window, select the appropriate guest tenant:
    
    ![Guest tenant](media/55237a5359fb66daf7bbb9413adab6b9.png "Guest tenant")
       
    > [!NOTE]
    > [!include[pn-teams](../includes/pn-teams.md)] might take a few seconds to reload.
    


## Make and take calls
### Accept a call  
When you see an incoming call notification in the bottom right of your screen, select Audio or Video to join the call.

### Make a one-to-one call to Remote Assist user in your company	
After launching Teams, select the Calls tab on your left to see suggested contacts. Select the Video icon on the contact card to call a suggested contact, of use the search bar to find a contact and call them. 

>![Note]
> Teams desktop users are not able to record a one-to-one call (i.e. an outgoing or incoming ad hoc call). To record a one-to-one call with a contact in your company or outside your company, a Teams desktop user must initiate the call using the Meet Now feature. (The Meet Now feature is not available for Teams mobile users.) Learn more about the Meet Now feature here. (include link to “Initiate and record a one-to-one call with Remote Assist HoloLens user using the Meet Now feature”)


### Make a one-to-one call to Remote Assist user outside your company	

You can make or receive a one-to-one call with a Remote Assist user from another company if external access for both companies has been enabled in Microsoft Teams. If you're the admin for your organization, to set up external access, see Set up cross-company calling. When searching for the external user, you must enter the full email address of the external user. 

>![Note]
> If you're not able to find the contact you're looking for, it might be because external access has not been enabled in Microsoft Teams for your company or the other company. Contact your administrator for help.  

### Make a group call (with Remote Assist HoloLens user only)

A group call can include up to 1 Remote Assist HoloLens user and 49 Teams Desktop users. 
Start by calling one person, and then select Open Participants ![Participants](media/RAHL_Participants.png "Participants") button. Then, search the person you would like to call and call them.


### Make and record a one-to-one call with a Remote Assist HoloLens user using the Meet Now feature 

You may want to record the Remote Assist call for documentation or record-keeping purposes. There are three ways to record a call. Learn about the different types of calls [here](insert link to “record a call”). 
Teams desktop only supports recording group calls and meetings (regardless of how many call participants are in the meeting). In other words, when you are in a call, a Teams desktop user can use Teams to initiate a cloud-based recording only if the call is a group call or a meeting. (At this time, a HoloLens user cannot record the call.) 
So how do you record a one-to-one call? You will need to make your one-to-one call a meeting. In other words, if you anticipate wanting to use Teams to create a cloud-based recording of a one-to-one call with a Remote Assist HoloLens user, the easiest way to do this is to initiate your call using the Teams **Meet Now** feature. (This effectively makes your ad hoc one-to-one call a meeting, and because Teams supports recording for meetings, you will be able record the call!)

1.	Navigate to the Calendar tab. On the top right corner of the page, you will see. Click **Meet Now.**
![MeetNow](media/PC_MeetNow.png "MeetNow")
2. Name the meeting and select **Join now**
3. Invite people to the meeting using the “Invite someone or dial a number” field on the right half of the screen. Click the […] and click start recording. 
4. When the call ends, it will appear as a normal Meeting in your Teams chat log. The chat log will include everyone was invited to the meeting. Stream processes the recording.
5. The person who initiates the recording is the recorder and owns the video. When a recording ends, it begins being uploaded to Microsoft Stream. Once the video is uploaded to Stream, the recorder receives an email notification, and all call participants can view a link to Stream via the Teams chat. The owner is the only participant who can [give permission](https://support.office.com/en-us/article/Play-and-share-a-meeting-recording-in-Teams-7d7e5dc5-9ae4-4b94-8589-27496037e8fa#bkmk_sharemeetingrecording) or [download the video](https://support.office.com/en-us/article/Play-and-share-a-meeting-recording-in-Teams-7d7e5dc5-9ae4-4b94-8589-27496037e8fa#bkmk_downloadmeetingrecording) to share the recording beyond these people. [Learn more about Stream video permissions.]( https://docs.microsoft.com/en-us/stream/portal-permissions)

You can find all the videos you own [here]( https://msit.microsoftstream.com/studio/videos).
If your admin has configured Field Service integration, you can access the recording link and can post it in a D365 Field Service booking.









## Working with annotations

Once [!include[pn-teams](../includes/pn-teams.md)] is installed, the expert can make video calls to (and receive them
from) contacts using [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] on a [!include[pn-hololens](../includes/pn-hololens.md)].

When in a call, the expert will see the contact’s space—including the
holograms—and can use the Mixed Reality toolbar in the video call window to add
holograms.

![Mixed Reality toolbar](media/071f358ab6bbf7c2072b15d9203a1593.png "Mixed Reality toolbar")

## Draw and annotate

### Edit mode

To start annotating a contact’s space, first do one of the following to pause
the video stream and enter edit mode:

-   Select anywhere in the call window.

-   Select one of the items on the Mixed Reality toolbar.

-   Select **Start editing**.

In edit mode, the expert will still see a live stream of the call in the corner
of the app window.

### Add arrows, ink, and files

Use the Mixed Reality toolbar to place arrows, draw, or add files:

-   To add arrows, select **Place arrow** ![Place arrow](media/6584f4b7932378aa23f6efbf460b304c.png "Place arrow") .

-   To add ink, select **Ink** ![Ink](media/187307e30fd713f5ae67aba854b78bc4.png "Ink") .

-   To change the arrow or ink color, select **Pick a color** ![Pick a color](media/5d9d3c70cf19ed175a8dc1ad71a60fc5.png "Pick a color") .

-   To add a file, select **Insert files** ![Insert files](media/41aa538d3be8e163215f7d9374abe90e.png "Insert files"), and then add an image file or a PDF file.

    > [!NOTE]
    > After adding them, images can’t be moved, deleted, or resized by the expert.

### Finish editing

When done annotating, do one of the following to finish editing and return to
live mode:

-   Select **Stop editing**.

-   Select the live video feed in the corner of your screen.

### Make changes to edits

To make changes to edits, do one of the following:

-   While in edit mode, select **Undo** to undo the last action.

-   While in edit mode, select **Erase all** ![Erase all](media/3aab547aa81003ad181eceadc2c83a47.png "Erase all") to erase all of the annotations made during that editing session.

-   While in live mode, select **Erase all** ![Erase all](media/3aab547aa81003ad181eceadc2c83a47.png "Erase all") to erase all of the annotations made during that call.

> [!NOTE]
> Specific drawings or arrows can’t be removed. Only the [!include[pn-hololens](../includes/pn-hololens.md)] user can make changes to or delete pictures added by an expert.

## Share your desktop or a running application with a Dynamics 365 Remote Assist user

When you share your desktop or running application with a [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] user, the user's video feed will change to a solid color. They'll still be able to use all the tools in the toolbar even though their video feed will no longer be displayed.

To share your desktop or a running application:

1. In [!include[pn-teams](../includes/pn-teams.md)], select the **Open share tray** button.

   ![Share tray button](media/share-tray.PNG "Share tray button")
   
2. Select the screen you want to share.

> [!NOTE]
> You can only share one application or screen at a time. If you want to share a different screen, select the **Close share tray** button to stop sharing, select a different screen, and then start sharing again.
