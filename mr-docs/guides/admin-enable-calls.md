---
author: prashantyvr
description: Learn how to enable or disable calling in a Dynamics 365 Guides environment 
ms.author: prashan
ms.date: 02/22/2024
ms.topic: how-to
title: Enable or disable calling for a Dynamics 365 Guides environment
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Enable or disable calling in a Dynamics 365 Guides environment

Calling in Microsoft Dynamics 365 Guides is enabled by default. When calling is enabled, a Dynamics 365 Guides HoloLens user can make or receive calls with a remote collaborator. The remote collaborator can join a call using Microsoft Teams desktop (PC or Mac) or the Teams mobile app. During the call, the remote collaborator can see everything seen by the Guides user, including holograms and the real world behind the holograms.

If you're an admin for Dynamics 365 Guides, enable or disable calling for users in a specific Dynamics 365 Guides environment. Enabling or disabling calling for a specific environment is useful:

- When operators or authors do not need to work with remote collaborators.

- You don't want HoloLens users to be able to inadvertently reveal proprietary information through a call.

[Learn about licensing requirements and limitations when making calls in Dynamics 365 Guides](requirements.md).

## Enable or disable calling

1. [Open the model-driven app](open-model-driven-app.md) in Guides.

1. On the bottom left side of the screen, select **Main**, and then select **Settings**.

   :::image type="content" source="media/main-to-settings-area.PNG" alt-text="Screenshot that shows changing from Main to Settings area in the Guides model-driven app.":::

1. In the left pane, select **Environment**, and then toggle **Enable Calling** on or off for this environment. This action enables or disables the functionality for all configured users signed into that environment. Disabling calling in a Dynamics 365 environment only disables that functionality for Guides and has no impact on that capability in Microsoft Teams.

   :::image type="content" source="media/enable-calling-mda.PNG" alt-text="Screenshot that shows enable and disable calling toggle in the Guides model-driven app.":::

If a user tries to start a call while working in an environment where calling is disabled, the user sees the following error message:

"**Your admin may have disabled calling or you may not have a Microsoft Teams or Remote Assist license.**"

> [!NOTE]
> Enabling or disabling calling is not immediate. A change can take time to propagate. [Learn how to revoke user access in an emergency in Microsoft Entra ID](/azure/active-directory/enterprise-users/users-revoke-access).

## See also

- [Make a call in Dynamics 365 Guides](make-call.md)
- [Licensing and product requirements for making calls in Dynamics 365 Guides](requirements.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
