---
title: Join a Dynamics 365 Remote Assist meeting on HoloLens
description: Learn how to join a Microsoft Teams meeting or live event in Dynamics 365 Remote Assist on HoloLens.
author:  BogdanBerg
ms.author: bogdanb
ms.date: 07/05/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
---

# Join a Dynamics 365 Remote Assist meeting on HoloLens

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

A [Microsoft Teams meeting](/microsoftteams/quick-start-meetings-live-events) is a meeting scheduled using Teams involving any number of participants. Meetings are useful for maintenance and repairs that are scheduled in advance. They're also useful for inspections and other recurring scenarios.

A [Microsoft Teams live event](/microsoftteams/teams-live-events/what-are-teams-live-events) is an extension of Teams meetings, enabling users to broadcast video and meeting content to a large online audience. These events are meant for one-to-many communications where the host of the event is leading the interactions and audience participation is primarily to view the content shared by host.

A Dynamics 365 Remote Assist HoloLens user can join a live event as a presenter or attendee in the same way they join a meeting.

Dynamics 365 Remote Assist doesn't support most of the features offered in [Microsoft Teams Premium](https://support.microsoft.com/en-us/office/overview-of-microsoft-teams-premium). Use of these features by another user, such as the meeting organizers, can cause problems in the meeting for the Remote Assist user.

> [!Note]
> If a remote collaborator joins a meeting, you will not receive a call or notification, regardless of whether you are in the app. You must select **Join Meeting** (or say "Remote Assist, Join meeting") to join the meeting. In addition, calling the participants involved in a scheduled meeting will not enable you to join the meeting; you must actually join the meeting.

If for some reason you're unable to join the meeting, you might also ask the Teams user to join the meeting and use the **Open Participants** feature to call you. An incoming call notification appears. Accept the call using audio or video, and you'll join the meeting.

![Screenshot of the HoloLens field of view, showing the join meeting option at the bottom.](media/02.03-contacts-meeting-notification.png "JoinMeeting")

> [!NOTE]
> Dynamics 365 Remote Assist users might not be able to join scheduled meetings between different companies if link-rewriting (URL-rewriting services) are used to fight spam. To make sure that users can join scheduled meetings in this situation, add an exception so that links from teams.microsoft.com are not rewritten.  

To join a meeting, select **Join Meeting**, or say "Remote Assist, Join Meeting", below the **Recent Contacts** screen. The **Join Meeting** button appears if the meeting is happening now or within the next 15 minutes. If your upcoming meetings overlap, you can use the arrows to select which meeting to join.  

After you join a meeting, you or the Teams user can add more people to the meeting. Select **Open Participants** (as represented by this icon: ![Graphic showing the open participants icon.](media/RAHL_Participants.png)). The first person you called appears on the left side of the video card, and a list of participants on the right side of the video card. On the bottom of the video card, there's a text field. Select the text field, and a holographic keyboard pops out. A list of your recent contacts appears. If the person you'd like to call isn't on the list, enter a name or email address using the holographic keyboard, and then select a name in the search results to start the call.

> [!NOTE]
> Dynamics 365 Remote Assist supports the Teams lobby on HoloLens. A HoloLens user can now admit a Teams guest into a meeting. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]
