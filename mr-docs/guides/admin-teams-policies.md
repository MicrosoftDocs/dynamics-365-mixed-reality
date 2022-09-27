# Teams policies supported by Dynamics 365 Guides

Microsoft Dynamics 365 Guides supports the following Microsoft Teams policies and capabilities:

- **Recording policy.** Turn off recordings for meetings and one-to-one calls.
- **Chat policy.** Turn off the ability to chat in meetings and one-to-one calls.
- **Video policy.** Remove access to video calls (calls are audio only).

## Turn off the ability to record calls

### For meetings

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Meeting policies**.
3. Create a new policy or edit an existing policy.
4. In the **Audio & video** section, turn off the **Allow cloud recording** setting. 

    ![Screenshot of Microsoft Teams admin center with Allow cloud recording setting highlighted.](media/calling-teams-policies-recording-meetings.JPG "Screenshot of Microsoft Teams admin center with Allow cloud recording setting highlighted")
    
5. Save the new or modified policy.
6. [Assign the policy to a user](#assign-a-policy-to-a-user).
7. Verify that the policy is working as expected in Teams desktop. 

### For one-to-one calls

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Voice** > **Calling policies**. 
3. Create a new policy or edit an existing policy.
4. Turn off the **Cloud recording for calling** setting. 

    ![Screenshot of Microsoft Teams admin center with Cloud recording for calling setting highlighted.](media/calling-teams-policies-recording-one-to-one.JPG "Screenshot of Microsoft Teams admin center with Cloud recording for calling setting highlighted")
    
5. Save the new or modified policy.
6. [Assign the policy to a user](#assign-a-policy-to-a-user).
7. Verify that the policy is working as expected in Teams desktop. 

## Turn off the ability to chat

### For meetings

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Meeting > Meeting policies**.
3. Create a new policy or edit an existing policy.
4. Scroll down to the **Participants & guests** section.
5. In the **Allow chat in meetings** field, select **Disabled**. 

    ![Screenshot of Microsoft Teams admin center with Allow chat in meetings field highlighted.](media/calling-teams-policies-chat-meetings.JPG "Screenshot of Microsoft Teams admin center with Cloud recording for calling setting highlighted")
    
5. Save the new or modified policy.
6. [Assign the policy to a user](#assign-a-policy-to-a-user).
7. Verify that the policy is working as expected in Teams desktop. 

### For one-to-one calls

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Messaging policies**.
3. Create a new policy or edit an existing policy.
4. Turn off the **Chat** setting. 

    ![Screenshot of Microsoft Teams admin center with Chat setting highlighted.](media/calling-teams-policies-chat-one-to-one.JPG "Screenshot of Microsoft Teams admin center with Chat setting highlighted")
    
5. Save the new or modified policy.
6. [Assign the policy to a user](#assign-a-policy-to-a-user).
7. Verify that the policy is working as expected in Teams desktop. 

## Turn off the ability to see video 

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Meetings > Meeting policies**.
3. Create a new policy or edit an existing policy.
4. In the **Audio & video** section:
    - In the **Mode for IP video** field, select **Disabled**.
    - Turn off the **Allow IP video** setting.

    ![Screenshot of Microsoft Teams admin center with Audio & video settings highlighted.](media/calling-teams-policies-video.JPG "Screenshot of Microsoft Teams admin center with Audio & video settings highlighted")
    
5. Save the new or modified policy.
6. [Assign the policy to a user](#assign-a-policy-to-a-user).
7. Verify that the policy is working as expected in Teams desktop.

## Policies for guest users

Users you [invite as guests](admin-add-guest-user.md) have limited scope of access by design. For example, guest users cannot start call recordings by default. You can restrict other access capabilities through policy. 

### Access guest policies

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Guest access**.
3. Create a new policy or edit an existing policy.
4. Make your changes.

    ![Screenshot of Microsoft Teams admin center showing Guest access settings.](media/calling-teams-policies-guest-access.JPG "Screenshot of Microsoft Teams admin center showing Guest access settings")

5. Save the new or modified policy.
6. [Assign the policy to a user](#assign-a-policy-to-a-user).
7. Verify that the policy is working as expected in Teams desktop.

## Assign a policy to a user

1. Go to https://admin.teams.microsoft.com/
2. On the left side of the screen, select **Users**, and then select the user you want to modify policies for.
3. Next to **Assigned policies**, select the **Edit** button.

    ![Screenshot of Microsoft Teams admin center with Edit button highlighted next to Assigned policies.](media/calling-teams-policies-edit.JPG "Screenshot of Microsoft Teams admin center with Edit button highlighted next to Assigned policies")
    
4. On the right side of the screen, in the **Meeting policy** and/or the **Messaging policy** fields, enter the name of the policy.

    ![Screenshot of Microsoft Teams admin center with Edit pane highlighted.](media/calling-teams-policies-edit-pane-settings.JPG "Screenshot of Microsoft Teams admin center with Edit pane highlighted")
    
5. Select **Apply**.
6. Verify that the policy is working as expected in Teams desktop.
