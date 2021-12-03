
# Restrict calling and the ability to access contacts in Dynamics 365 Remote Assist

If you [have a scenario where you need to protect company information](restricted-mode-overview.md) from Dynamics 365 Remote Assist HoloLens users, you can restrict the ability to:

- Initiate calls 
- Receive incoming calls
- Access contacts

You can do this without affecting the ability to join meetings or receive meeting notifications (in advance or while a meeting is already underway), so users can continue to use Dynamics 365 Remote Assist to troubleshoot issues with colleagues. 

> [!NOTE]
> You can't restrict calling for the Dynamics 365 Remote Assist mobile app, but you can [set up one-time calls with the mobile app](one-time-call.md). 

## Restrict calling

> [!NOTE]
> You must have Microsoft Teams admin privileges to restrict calling in Dynamics 365 Remote Assist.

You can restrict calling by creating a new Microsoft Teams policy, and then assign that policy to the appropriate users. 

> [!TIP]
> You can also assign policies to groups. [Learn more](https://docs.microsoft.com/microsoftteams/assign-policies-users-and-groups) 

1. Go to the [Microsoft Teams admin center](https://admin.teams.microsoft.com) and sign in with your admin credentials.      

2. In the left pane, select **Calling policies**, and then select **Add**.

    ![Screenshot of Microsoft Teams admin center with Calling policies command and Add button highlighted.](media/restricted-mode-calling-add-policy.jpg "Screenshot of Microsoft Teams admin center with Calling policies command and Add button highlighted")

3. Enter a name for your policy, turn **Make private calls** to **Off**, and then select **Save**. 

    ![Screenshot highlighting description, Make private calls option, and Save button.](media/restricted-mode-calling-turn-off-private-calls.jpg "Screenshot highlighting description, Make private calls option, and Save button")

4. In the left pane, select **Manage users**, and then select the user you want to assign the policy to. IS IT THE USER OR A POLICY YOU'RE SELECTING HERE?

    ![Screenshot highlighting Manage users command and selected policy.](media/restricted-mode-calling-assign-user.jpg "Screenshot highlighting Manage users command and selected policy")

5. Select the **Policies** button, and then select **Edit**.

    ![Screenshot highlighting Policies button and Edit button.](media/restricted-mode-calling-edit.jpg "Screenshot highlighting Policies button and Edit button")

6. On the right side of the screen, in the **Calling policy** list, select the policy you created, and then select **Apply**.

    ![Screenshot of Calling policy list opened.](media/restricted-mode-calling-select-policy.jpg "Screenshot of Calling policy list opened")

   Once the policy takes effect, users will be able to join notifications or receive notifications for meetings but they won't be able to initiate calls or receive calls if they're not in a meeting. They also won't be able to access the contacts list. 

    > [!NOTE]
    > It can take a few hours before the policy assignments go into effect.

    
