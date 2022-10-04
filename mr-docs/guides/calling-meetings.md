---
title: 
author: 
description: 
ms.author: 
ms.date: 10/04/2022
ms.topic: article
ms.reviewer: v-bholmes
---

# Join a Microsoft Teams meeting from Dynamics 365 Guides

You can join a Microsoft Teams meeting from Dynamics 365 Guides on HoloLens. A [Microsoft Teams meeting](/microsoftteams/quick-start-meetings-live-events) is a meeting **scheduled** with Teams that includes any number of participants. 

It's also possible to join a [Microsoft Teams live event](/microsoftteams/teams-live-events/what-are-teams-live-events) from Dynamics 365 Guides, but this scenario is not officially supported.  

> [!IMPORTANT] 
> To join a meeting from Dynamics 365 Guides on HoloLens, you must have an Exchange Online license (not Exchange on-premises). 

## Join a scheduled meeting

1. Look at the palm of your hand to open the Main menu, and then select the **Communications** button.

    ![Screenshot of Communications button on Main menu.](media/calling-meetings-1.JPG "Screenshot of Communications button on Main menu")
    
2. Select **Meetings**.

    ![Screenshot highlighting Meetings button.](media/calling-meetings-2.JPG "Screenshot highlighting Meetings button")

    The Meeting window opens to the current day so you can see all of your meetings for that day. 

    ![Screenshot of calendar in Meetings window.](media/calling-meetings-3.JPG "Screenshot of calendar in Meetings window")

    > [!NOTE]
    > Dynamics 365 Guides supports the default calendar only. You can't change the layout of the calendar to the day, week, or month view, and you can't substitute a user's secondary calendar (for vacations or team-wide events, for example). 

    To change to a different day, select the day at the top of the screen. To switch to a different week, use the arrows in the upper right-corner of the screen. To go back to the current day at any time, select **Today** at the top of the screen. 
    
3. To open a specific meeting, select the meeting on the calendar. In the window that appears, you'll see the meeting details, including the meeting date and time, meeting name, and organizer. 

    ![Screenshot of Meeting details window.](media/calling-meetings-6.JPG "Screenshot of Meeting details window")

4. Select **Join** to join the meeting. 

    When a participant joins the meeting, their avatar is displayed in the upper-right corner of the Meeting window. 

    ![Screenshot of Meeting window before participants join.](media/calling-meetings-8.JPG "Screenshot of Meeting window before participants join")
    
## Add a participant from your organization to the meeting

To add a participant from your organization that wasn't included in the original invite:

1. Select the **Open Participants** button.

    ![Screenshot highlighting Open Participants button.](media/calling-start-call-4.JPG "Screenshot highlighting Open Participants button")

2. In the Participants area (to the right of the video feed), select the **Participants** button. This opens the **Recent** list.
    
    ![Screenshot highlighting Participants button in Participants area.](media/calling-start-call-5.JPG "Screenshot highlighting Participants button in Participants area")

3. Do one of the following:

    - If the contact you want to add is listed in the **Recent** list, select the contact's tile, and then select **Show video**.

    - If the contact isn't listed in the **Recent** list, place your cursor in the **Search** box, and then in the holographic keyboard that appears, enter the person's name or email address. Use the **Microphone** button if you prefer to use your voice to enter the person's name in the **Search** box. 

      ![Screenshot of Recent list with Search box and holographic keyboard showing.](media/calling-start-call-6.JPG "Screenshot of Recent list with Search box and holographic keyboard showing")

## Admit a participant from outside your organization

> [!NOTE]
> Dynamics 365 Guides users might not be able to join scheduled meetings between different companies if link-rewriting (URL-rewriting services) are used to fight spam. To make sure that users can join scheduled meetings in this situation, add an exception so that links from teams.microsoft.com are not rewritten. 
    
If a participant wants to join the meeting, but they're not part of your organization, a notification appears at the top of the Meeting window to let you know that the participant is waiting in the lobby. A **Participants** button with a red dot (showing action required) appears in the bottom-right corner of the Meeting window. 

![Screenshot showing notification that someone is waiting in the Lobby.](media/calling-meetings-10.JPG "Screenshot showing notification that someone is waiting in the lobby")
    
To admit or decline the participant:

- Select the **Open Participants** button below the video feed to display the participant tiles on the right of the screen. In the first participant tile, select **Admit** or **Decline**. 

> [!NOTE]
> The meeting organizer can decide who is admitted into a meeting directly and who has to wait for someone to admit them. [Learn more about choosing who can bypass the lobby](https://support.microsoft.com/en-us/office/change-participant-settings-for-a-teams-meeting-53261366-dbd5-45f9-aae9-a70e6354f88e). 

## Schedule and join a meeting from Teams desktop (PC or Mac)

> [!NOTE]
> Dynamics 365 Guides users might not be able to join scheduled meetings between different companies if link-rewriting (URL-rewriting services) are used to fight spam. To make sure that users can join scheduled meetings in this situation, add an exception so that links from teams.microsoft.com are not rewritten.  

### Schedule a meeting ahead of the call

Check out the following links:

- [Schedule a meeting in Teams](https://support.office.com/article/Schedule-a-meeting-in-Teams-943507a9-8583-4c58-b5d2-8ec8265e04e5#ID0EAABAAA=Desktop)

- [Watch a video on managing Teams meetings](https://support.office.com/article/Video-Manage-meetings-ba44d0fd-da3c-4541-a3eb-a868f5e2b137)

### Join a Teams meeting

Check out the following links:

- [Join a meeting in Teams](https://support.office.com/article/join-a-meeting-in-teams-1613bb53-f3fa-431e-85a9-d6a91e3468c9)

- [Watch a video on joining a Teams meeting](https://support.office.com/article/join-a-teams-meeting-078e9868-f1aa-4414-8bb9-ee88e9236ee4?ui=en-US&rs=en-US&ad=US)

If the Dynamics 365 Guides user is invited to the meeting, they can sign in to Dynamics 365 Guides, and then select **Join Meeting** at the bottom of the **Recent Contacts** page.

If the Dynamics 365 Guides user is not invited to the meeting, but you would like them to join the meeting: 

1. Join the meeting, and then select **Participants** from the **Call Controls** toolbar.

2. Start typing their name, and then call them. 

[!INCLUDE[footer-include](../includes/footer-banner.md)]
