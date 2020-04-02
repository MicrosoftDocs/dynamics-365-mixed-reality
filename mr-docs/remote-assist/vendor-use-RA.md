---
author: sopsun
description: Vendors and contractors use Remote Assist
ms.author: sophiasysun
ms.date: 04/01/2020
ms.service: crm-online
ms.topic: article
title: Vendors and contractors use Remote Assist
ms.reviewer: krbjoran
---

# Vendors and contractors use Remote Assist

## Introduction

A Remote Assist call involves one party (technician) using Remote Assist and the other using Teams (expert or remote collaborator).  In most cases, technician and remote collaborators all belong to the same tenant, and thus a [standard deployment of Remote Assist](deploy-remote-assist.md) and [standard deployment of Teams](set-up-teams.md) is all you need. 

However, there are certain scenarios where this may not be the case: 

1. **Scenario 1: Multi-tenant company deployments,** i.e., a company has a multi-tenant configuration across different organizations or business units. [Learn more about this scenario.](multi-tenant-deployment.md) 

1. **Scenario 2: Vendors and contractors use Remote Assist,** i.e., a company wants vendors and contractors that aren’t part of the company tenant to use Remote Assist. This document focuses on scenario 2.

>[!NOTE]
>This article is intended for administrators, and assumes that you have Microsoft Teams **AND** Azure Active Directory (Azure AD) admin privileges. You should also be familiar with the [Teams admin portal](https://admin.teams.microsoft.com/).

## Account types

Throughout this article, we'll be referring to a few account types: 

1. **Internal account**: An Azure Active Directory (Azure AD) account that is created inside your tenant for internal users.
2. **Service account**: An Azure AD account that is created inside your tenant for users who are not currently part of your tenant.\

## Scenario overview

> [!Note] To appropriately license this scenario, please contact your Microsoft sales representative to license.

Companies frequently want to leverage non-company employees such as vendors or contractors to perform specific service tasks. In this case, companies still handle all license configuration, but want to enable their vendors or contractors to seamlessly use Remote Assist to collaborate with them. 

### Example

Company ABC uses Tenant ABC. Tenant ABC has users who want to use Teams to remotely collaborate with company vendors and contractors. Some of these vendors and contractors are in an existing tenant and others are not. Company ABC wants to give vendors and contractors Remote Assist licenses so they can use it for their daily service tasks. This scenario is depicted in Figure 2.1 

In Figure 1.1, Company ABC used Azure AD to create **service accounts** (SAs) inside Tenant ABC. Tenant ABC administrator assigned a Remote Assist license (Jason - anything else?) to each service account. Service account credentials were then distributed to company vendors and contractors.
* Bob@Contoso1.com is still a member of Contoso1, and now uses SA1@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.
* Toni@Contoso1.com is still a member of ContosoN, and now uses SA2@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.
* User@Outlook.com was not a member of any other tenant - that contractor uses a regular personal email (e.g. @outlook.com) for work. Now, user@outlook.com users SA3@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.

**Figure 1.1**
![Diagram showing Tenant A providing a Remote Assist license to users outside of Tenant A.](media/cross-tenant-licensing.png)

>[!Note] If Tenant ABC does not configure information barriers, any service account user can search for and communicate with any other service account user or internal account user in Tenant ABC. Information barriers are a great way to control who can search and collaborate with one another when using Microsoft Teams and Remote Assist. Learn more about information barriers and how to configure them [here](https://docs.microsoft.com/en-us/microsoft-365/compliance/information-barriers?view=o365-worldwide).

>[!Note] Because Teams users and Remote Assist users are all in Tenant ABC, they can each search for users they are allowed to search for by typing that user's name, rather than typing their entire email address.

### Implementation

1. Determine if information barriers are necessary

Information barrier policies determine and prevent the following kinds of unauthorized communications between users who have Azure AD accounts in a tenant:

- Searching for a user
- Adding a member to a team
- Starting a chat session with someone
- Starting a group chat
- Inviting someone to join a meeting
- Sharing a screen
- Placing a call

2. If information barriers are necessary, plan how you segment users. 

You can segment users based on different attributes, such as what department they belong to, what Azure AD group they are a member of, or even by their usage location. A full list of attributes can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide#reference). To see how an organization might approach defining segments and policies, consider the following [example](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide#example-contosos-departments-segments-and-policies). A downloadable Excel workbook is available to help you plan and define your segments and policies (and create your PowerShell cmdlets). [Get the workbook.](https://github.com/MicrosoftDocs/OfficeDocs-O365SecComp/raw/public/SecurityCompliance/media/InfoBarriers-PowerShellGenerator.xlsx). Additional information about information barriers can be found [here].

3. Buy the correct licenses

Learn about [licenses required to use Remote Assist](requirements.md).

If you would like to control who the service account user can search and collaborate with, you will need to assign the service account a information barrier license. The following licensing suites include information barrier licenses:

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

For more information, see [Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)

4. [Create service accounts](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory).

5. [Assign licenses](https://docs.microsoft.com/azure/active-directory/fundamentals/license-users-groups) to each service account user. 

6. If information barriers are necessary, [configure information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide).
