---
author: davepinch
description: Learn how to add a guest user (partner, vendor, supplier, or consultant) in Dynamics 365 Guides
ms.author: davepinch
ms.date: 08/09/2022
ms.topic: article
title: Add a guest user in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Add a guest user in Dynamics 365 Guides

Anyone who is not part of a Microsoft Dynamics 365 Guides organization, but has an Azure Active Directory account, can be added as a guest user by a global admin. The user can then access Dynamics 365 Guides content in that organization as an operator. A "guest" is defined as someone who doesn't have a school or work account with the organization. For example, a guest could be a partner, vendor, supplier, or consultant. 

> [!NOTE]
> Anyone with a consumer email account (for example, an Outlook.com or Gmail.com account) can be a guest user in Azure Active Directory, but users with these types of email accounts are not supported as guest users in Dynamics 365 Guides. 

To add a user as a guest, you [invite them as a guest to Microsoft Teams, or create a guest account for them in Azure Active Directory](https://docs.microsoft.com/microsoft-365/admin/add-users/about-guest-users?view=o365-worldwide). Guest users are covered by the same compliance and auditing protection as other Microsoft 365 users. Guest access is subject to Azure Active Directory and Microsoft 365 service limits.

The guest experience has limitations by design. For a full list of what a guest can and can't do in Teams, see [Guest access in Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-experience). 

> [!IMPORTANT]
> A Microsoft Teams admin can [configure Teams to block guest users](https://docs.microsoft.com/microsoftteams/set-up-guests), but Dynamics 365 Guides ignores that configuration and allows guest users to make calls from HoloLens. 

## Guest user management

When a guest is invited to join an organization, they receive a welcome email message. This message includes some information about the organization and what to expect as a member. The guest must accept the invitation by selecting **Accept Invitation** in the email message before they can access the organization and the organization's guides.

> [!NOTE]
> After a guest is added to an organization, it may take a few hours before they have access.    

When a user joins an organization as a guest, a **(Guest)** label appears next to their name so everyone in the organization can easily identify guests. 

## Restrict guests from searching for a user in your organization

Some organizations might want to restrict guest access to prevent guests from starting a chat or a call by searching for a user in the directory. This restriction is controlled in the **External collaboration settings** section of the Azure Active Directory admin center. For details, see [Restrict guest access permissions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/users-restrict-guest-permissions).

- To restrict guest users from searching for a user in your organization, in the **Guest user access** section, select the **Guest users have limited access to properties and memberships of directory objects** option.

- To allow guest users to search for a user in your organization, select the **Guest users have the same access as members (most inclusive)** option. 

## Comparison of team member and guest capabilities

Dynamics 365 Guides is a Microsoft Teams client. Dynamics 365 Guides calling, chat, file share, and meeting functions (if available) are based on Teams. Guest user capabilities in Dynamics 365 Guides also match those available in Teams. Global admins control guest user access for the calling, chat, file sharing and meeting features available to an organization's guests by assigning or removing a Team's license for the guest user. For more information, see [Use guest access and external access to collaborate with people outside your organization](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations). This article includes a [table that compares Teams functionality available for an organization's team members and its guests](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#external-access-external-chat-and-meetings). 

The **Guest user access restrictions** policy in Azure Active Directory determines permissions for guests in your directory. The following table describes the three policy options.

|Policy option|Description|
|-------------------------------------------------------|---------------------------------------------------------------------------------------|
|**Guest users have the same access as members (most inclusive)**|Guests have the same access to directory data as regular users in your directory.|
|**Guest users have limited access to properties and membership of directory objects**|Guests don't have permissions for certain directory tasks, such as enumerating users, groups, or other directory resources using Microsoft Graph.|
|**Guest user access is restricted to properties and memberships of their own directory objects (most restrictive)**|Guests can only access their own directory objects.|

To learn more, see [What are the default user permissions in Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions)

## See also

- [Use guest access and external access to collaborate with people outside your organization](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations)
- [Quickstart: Add a guest user and send an invitation](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)
- [Leave an organization as a B2B collaboration user](https://docs.microsoft.com/azure/active-directory/b2b/leave-the-organization)
