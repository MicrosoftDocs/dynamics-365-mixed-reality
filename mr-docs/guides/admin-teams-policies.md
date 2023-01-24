---
author: Mamaylya
description: Learn about the Microsoft Teams policies supported by Dynamics 365 Guides
ms.author: mamaylya
ms.date: 01/20/2023
ms.topic: article
title: Manage Teams policies supported by Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Manage Teams policies supported by Dynamics 365 Guides

Microsoft Dynamics 365 Guides supports the following Microsoft Teams policies and capabilities:

- **Recording policy.** Turn off recordings for meetings and one-to-one calls.
- **Chat policy.** Turn off the ability to chat in meetings and one-to-one calls.
- **Video policy.** Remove ability to share video calls (calls are audio only).

## Turn off the ability to record calls

When you turn off the ability to record calls, the **Recording** button is unavailable.

![Screenshot of Call window with Recording button disabled.](media/calling-teams-policies-recording-disabled.JPG "Screenshot of Call window with Recording button disabled")

> [!NOTE]
> By default, [Guest users](admin-add-guest-user.md) cannot record calls.

### Turn off the ability to record in meetings

1. Go to https://admin.teams.microsoft.com/
1. On the left side of the screen, select **Meetings > Meeting policies**.
1. Create a new policy or edit an existing policy.
1. In the **Recording & transcription** section, turn off the **Cloud recording** setting.

    ![Screenshot of Microsoft Teams admin center with Allow cloud recording setting highlighted.](media/calling-teams-policies-recording-meetings.JPG "Screenshot of Microsoft Teams admin center with Allow cloud recording setting highlighted")

1. Save the new or modified policy.
1. [Assign the policy to individual users or groups](/microsoftteams/assign-policies-users-and-groups).
1. Verify that the policy is working as expected in Teams desktop.

### Turn off the ability to record in one-to-one and group calls

1. Go to https://admin.teams.microsoft.com/
1. On the left side of the screen, select **Voice** > **Calling policies**.
1. Create a new policy or edit an existing policy.
1. Turn off the **Cloud recording for calling** setting. 

    ![Screenshot of Microsoft Teams admin center with Cloud recording for calling setting highlighted.](media/calling-teams-policies-recording-one-to-one.JPG "Screenshot of Microsoft Teams admin center with Cloud recording for calling setting highlighted")

1. Save the new or modified policy.
1. [Assign the policy to individual users or groups](/microsoftteams/assign-policies-users-and-groups).
1. Verify that the policy is working as expected in Teams desktop.

## Turn off the ability to chat

When you turn off the ability to chat, the HoloLens user sees the "Chat is unavailable" message in the chat message box.

![Screenshot of Chat window with chat messaging disabled.](media/calling-teams-policies-chat-disabled.JPG "Screenshot of Chat window with chat messaging disabled")

### Turn off the ability to chat in meetings

1. Go to https://admin.teams.microsoft.com/
1. On the left side of the screen, select **Meetings > Meeting policies**.
1. Create a new policy or edit an existing policy.
1. Scroll down to the **Participants & guests** section.
1. In the **Chat in meetings** field, select **Turn it off for everyone**.

    ![Screenshot of Microsoft Teams admin center with Allow chat in meetings field highlighted.](media/calling-teams-policies-chat-meetings.JPG "Screenshot of Microsoft Teams admin center with Allow chat in meetings field highlighted")

1. Save the new or modified policy.
1. [Assign the policy to individual users or groups](/microsoftteams/assign-policies-users-and-groups).
1. Verify that the policy is working as expected in Teams desktop.

### Turn off the ability to chat in one-to-one and group calls

1. Go to https://admin.teams.microsoft.com/
1. On the left side of the screen, select **Messaging policies**.
1. Create a new policy or edit an existing policy.
1. Turn off the **Chat** setting.

    ![Screenshot of Microsoft Teams admin center with Chat setting highlighted.](media/calling-teams-policies-chat-one-to-one.JPG "Screenshot of Microsoft Teams admin center with Chat setting highlighted")

1. Save the new or modified policy.
1. [Assign the policy to individual users or groups](/microsoftteams/assign-policies-users-and-groups).
1. Verify that the policy is working as expected in Teams desktop.

## Turn off the ability to share video

When you turn off the ability to share video, the **Video** button is unavailable.

![Screenshot of Call window with Video button disabled.](media/calling-teams-policies-video-disabled.JPG "Screenshot of Call window with Video button disabled")

### Turn off video

1. Go to https://admin.teams.microsoft.com/
1. On the left side of the screen, select **Meetings > Meeting policies**.
1. Create a new policy or edit an existing policy.
1. In the **Audio & video** section:
    - In the **Mode for IP video** field, select **Not enabled**.
    - Turn off the **IP video** setting.

    ![Screenshot of Microsoft Teams admin center with Audio & video settings highlighted.](media/calling-teams-policies-video.JPG "Screenshot of Microsoft Teams admin center with Audio & video settings highlighted")

1. Save the new or modified policy.
1. [Assign the policy to individual users or groups](/microsoftteams/assign-policies-users-and-groups).
1. Verify that the policy is working as expected in Teams desktop.

## Policies for guest users

Users you [invite as guests](admin-add-guest-user.md) have limited scope of access by design. For example, guest users cannot start call recordings by default. You can restrict other access capabilities through policy. 

### Access guest policies

1. Go to https://admin.teams.microsoft.com/
1. On the left side of the screen, select **Guest access**.
1. Create a new policy or edit an existing policy.
1. Make your changes.

    ![Screenshot of Microsoft Teams admin center showing Guest access settings.](media/calling-teams-policies-guest-access.JPG "Screenshot of Microsoft Teams admin center showing Guest access settings")

1. Save the new or modified policy.
1. [Assign the policy to individual users or groups](/microsoftteams/assign-policies-users-and-groups).
1. Verify that the policy is working as expected in Teams desktop.

## FAQ on Teams policies

### Can a policy be applied to a device or an app?

No, policies can only be applied to users or groups.

### Do one-to-one policies also apply to group calls?

Yes, one-to-one policies also apply to group calls, but meetings have their own policy.

### When are policies applied

Policies are applied when the user signs in. After making a policy change, the user will need to sign out and back in or close and open the app to apply the policy change. 

