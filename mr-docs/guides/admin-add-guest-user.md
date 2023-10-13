---
author: davepinch
description: Learn how to invite a guest user to operate a guide in Microsoft Dynamics 365 Guides
ms.author: davepinch
ms.date: 04/28/2023
ms.topic: article
title: Invite a guest user to operate a guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Invite a guest user to operate a guide in Dynamics 365 Guides

Anyone who is not part of a Microsoft Dynamics 365 Guides organization, but has an Azure Active Directory account, can be added as a guest user by a global admin. The user can then access Dynamics 365 Guides content in that organization **as an operator.** A "guest" is defined as someone who doesn't have a school or work account with the organization. For example, a guest could be a partner, vendor, supplier, or consultant. 

## Invite a guest

To add a guest user, you [invite them as a guest to Microsoft Teams, or create a guest account for them in Azure Active Directory](/microsoft-365/admin/add-users/about-guest-users).

When a guest is invited to join an organization, they receive a welcome email message. This message includes some information about the organization and what to expect as a member. The guest must accept the invitation by selecting **Accept Invitation** in the email message before they can access the organization and the organization's guides.

You must also [assign a Dynamics 365 Guides license](/microsoft-365/admin/manage/assign-licenses-to-users) and [assign user roles](assign-role.md) to the added guest accounts. Guest users are covered by the same compliance and auditing protection as other Microsoft 365 users. Guest access is subject to Azure Active Directory and Microsoft 365 service limits.

Your network admin needs to include an additional endpoint to [the IP addresses and/or endpoints that are required to connect to the Dynamics 365 servers](admin-network-requirements.md).

> [!NOTE]
> After a guest is added to an organization, it may take a few hours before they have access.    

When a user joins an organization as a guest, a **(Guest)** label appears next to their name so everyone in the organization can easily identify guests. 

## Limitations

- The guest calling experience has limitations by design. For a full list of what a guest can and can't do in Teams, see [Guest calling experience in Teams](/microsoftteams/guest-experience).

- The Dynamics 365 Guides PC app does not support guest access. 

- Guest users cannot record calls in the HoloLens app.

- Anyone with a consumer email account (for example, an Outlook.com or Gmail.com account) can be a guest user in Azure Active Directory, but users with these types of email accounts are not supported as guest users in Dynamics 365 Guides. 

## Restrict guests from searching when making calls in Dynamics 365 Guides

Some organizations might want to restrict guest access to prevent guests from starting a chat or a call by searching for a user in the directory. This restriction is controlled in the **External collaboration settings** section of the Azure Active Directory admin center. For details, see [Restrict guest access permissions in Azure Active Directory](/azure/active-directory/enterprise-users/users-restrict-guest-permissions).

- To restrict guest users from searching for a user in your organization, in the **Guest user access** section, select the **Guest users have limited access to properties and memberships of directory objects** option.

- To allow guest users to search for a user in your organization, select the **Guest users have the same access as members (most inclusive)** option.

## Comparison of team member and guest capabilities

Dynamics 365 Guides is a Microsoft Teams client. Dynamics 365 Guides calling is based on Teams. Guest user capabilities in Dynamics 365 Guides also match those available in Teams. Global admins control guest user access for the calling features available to an organization's guests by assigning or removing a Team's license for the guest user. For more information, see [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations). This article includes a [table that compares Teams functionality available for an organization's team members and its guests](/microsoftteams/communicate-with-users-from-other-organizations#external-access-external-chat-and-meetings). See also [Collaborate with guests in a team](/microsoft-365/solutions/collaborate-as-team).

The **Guest user access restrictions** policy in Azure Active Directory determines permissions for guests in your directory. The following table describes the three policy options.

|Policy option|Description|
|-------------------------------------------------------|---------------------------------------------------------------------------------------|
|**Guest users have the same access as members (most inclusive)**|Guests have the same access to directory data as regular users in your directory.|
|**Guest users have limited access to properties and membership of directory objects**|Guests don't have permissions for certain directory tasks, such as enumerating users, groups, or other directory resources using Microsoft Graph.|
|**Guest user access is restricted to properties and memberships of their own directory objects (most restrictive)**|Guests can only access their own directory objects.|

To learn more, see [What are the default user permissions in Azure Active Directory?](/azure/active-directory/fundamentals/users-default-permissions)

See also [Teams policies supported by Dynamics 365 Guides](admin-teams-policies.md).

> [!NOTE]
> Guests cannot start recordings in Teams calls. 

## See also

- [Use guest access and external access to collaborate with people outside your organization](/microsoftteams/communicate-with-users-from-other-organizations)
- [Quickstart: Add a guest user and send an invitation](/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)
- [Leave an organization as an external user](/azure/active-directory/b2b/leave-the-organization)
