---
author: davepinch
description: Learn how to enable or disable calling in a Dynamics 365 Guides environment 
ms.author: davepinch
ms.date: 04/28/2023
ms.topic: how-to
title: Enable or disable calling for a Dynamics 365 Guides environment
ms.reviewer: v-wendysmith
---

# Enable or disable calling in a Dynamics 365 Guides environment

Calling in Microsoft Dynamics 365 Guides is enabled by default. When calling is enabled, a Dynamics 365 Guides HoloLens user can make or receive calls with a remote collaborator. The remote collaborator can join a call using Microsoft Teams desktop (PC or Mac) or the Teams mobile app. During the call, the remote collaborator can see everything seen by the Dynamics 365 Guides user, including holograms and the real world behind the holograms.

If you're an admin for Dynamics 365 Guides, enable or disable calling for users in a specific Dynamics 365 Guides environment. Enabling or disabling calling for a specific environment is useful:

- When operators or authors do not need to work with remote collaborators.

- You don't want HoloLens users to be able to inadvertently reveal proprietary information through a call.

[Learn about licensing requirements and limitations when making calls in Dynamics 365 Guides](requirements.md)

## Enable or disable calling

1. Sign in to the environment by using your admin or author credentials.

    > [!TIP]
    > To find the URL for the environment, select the **Analyze** tab in the PC app. The URL is shown in the **Environment URL** field at the bottom of the page. Copy this URL, and paste it into the address bar of your web browser.
    >
    > ![Environment URL field.](media/environment-url.PNG "Environment URL field")

2. In Power Apps, select the **Guides** app tile.

    ![Guides app tile.](media/guides-app-tile.PNG "Guides app tile")

3. In the left pane, use the area picker at the bottom of the screen to switch the area selection from **Main** to **Settings** to view all settings for the environment.

    ![Settings highlighted in the left pane.](media/admin-enable-calling-settings.JPG "Settings highlighted in left pane")

4. In the left pane, select **Environment**, and then move the **Enable Calling** slider as needed to enable or disable calling for the environment. This action enables or disables the functionality for all configured users signed into that environment. Disabling calling in a Dynamics 365 environment only disables that functionality for Guides and has no impact on that capability in Microsoft Teams.

    ![New command highlighted at top of Power Apps screen.](media/admin-enable-calling.JPG "New command highlighted at top of Power Apps screen")

    If a user tries to start a call while working in an environment where calling is disabled, the user will see the following error message:

    "**Your admin may have disabled calling or you may not have a Microsoft Teams or Remote Assist license.**"

    > [!NOTE]
    > Enabling or disabling calling is not immediate. A change can take time to propagate. [Learn how to revoke user access in an emergency in Azure Active Directory](/azure/active-directory/enterprise-users/users-revoke-access).

## See also

- [Make a call in Dynamics 365 Guides](make-call.md)
- [Licensing and product requirements for making calls in Dynamics 365 Guides](requirements.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
