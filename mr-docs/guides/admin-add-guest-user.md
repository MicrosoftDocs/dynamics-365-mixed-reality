---
author: prashantyvr
description: Learn how to invite a guest user to operate a guide in Microsoft Dynamics 365 Guides.
ms.author: prashan
ms.date: 04/24/2024
ms.topic: how-to
title: Invite a guest user to operate a guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Invite a guest user to operate a guide in Dynamics 365 Guides

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

Anyone who isn't part of a Microsoft Dynamics 365 Guides organization, but has a Microsoft Entra account, can be added as a guest user. The user can then access Dynamics 365 Guides content in that organization **as an operator.** A "guest" is defined as someone who doesn't have a school or work account with the organization. For example, a guest could be a partner, vendor, supplier, or consultant.

## Limitations

- The guest calling experience has limitations by design. For a full list of what a guest can and can't do in Teams, see [Guest calling experience in Teams](/microsoftteams/guest-experience).

- The Dynamics 365 Guides PC app doesn't support guest access.

- Guest users can't record calls in the HoloLens app.

- Anyone with a consumer email account (for example, an Outlook.com or Gmail.com account) can be a guest user in Microsoft Entra, but users with these types of email accounts aren't supported as guest users in Dynamics 365 Guides.

## Invite a guest

1. [Invite the user as a guest to Microsoft Teams, or create a guest account for them in Microsoft Entra admin center](/entra/fundamentals/add-users#add-a-new-guest-user).

   The guest user receives a welcome email message that includes some information about the organization and what to expect as a member. The guest must accept the invitation by selecting **Accept Invitation** in the email message before they can access the organization and the organization's guides.

1. [Assign a Dynamics 365 Guides license](/microsoft-365/admin/manage/assign-licenses-to-users) and [assign user roles](assign-role.md) to the added guest accounts. Guest users are covered by the same compliance and auditing protection as other Microsoft 365 users. Guest access is subject to Microsoft Entra ID and Microsoft 365 service limits.

1. Ask your network admin to include another endpoint to [the IP addresses and/or endpoints that are required to connect to the Dynamics 365 servers](admin-network-requirements.md).

> [!NOTE]
> After a guest is added to an organization, it may take a few hours before they have access.

When a user joins an organization as a guest, a **(Guest)** label appears next to their name so everyone in the organization can easily identify guests.

## Restrict guests from searching when making calls in Dynamics 365 Guides

Some organizations might want to restrict guest access to prevent guests from starting a chat or a call by searching for a user in the directory.

1. [Restrict guest access permissions in Microsoft Entra ID](/entra/identity/users/users-restrict-guest-permissions).

1. On the **External collaboration settings** page, make your selection in the **Guest user access** section:

   - To restrict guest users from searching for a user in your organization, select the **Guest users have limited access to properties and memberships of directory objects** option.

   - To allow guest users to search for a user in your organization, select the **Guest users have the same access as members (most inclusive)** option.

## See also

- [Teams policies supported by Dynamics 365 Guides](admin-teams-policies.md)
- [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations)
- [What are the default user permissions in Microsoft Entra ID?](/azure/active-directory/fundamentals/users-default-permissions)
