---
author: pawinfie
description:  Technical document for deploying cross-tenant or cross-company Remote Assist calls
ms.author: pawinfie
ms.date: 03/24/2020
ms.service: crm-online
ms.topic: article
title: Cross-tenant Remote Assist licensing implementation
ms.reviewer: krbjoran
---

# How to Lease Remote Assist licenses to external users

This document assumes that you have read our [Remote Assist External Collaboration Scenarios](out-of-tenant-overview.md) document. 

Information barriers aren't just about collaborating but also searching. In Microsoft Teams, information barrier policies determine and prevent the following kinds of unauthorized communications:

- Searching for a user
- Adding a member to a team
- Starting a chat session with someone
- Starting a group chat
- Inviting someone to join a meeting
- Sharing a screen
- Placing a call

Additional information about Information Barriers can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#what-happens-with-information-barriers).

>[!NOTE]
> This article assumes that you have read the article [Remote Assist cross-tenant communication](cross-tenant-overview.md). If you haven't, please review that article first.

In this article, we'll take a look at how to implement licensing across multiple Remote Assist tenants through the following steps:

1. Determine if information barriers are necessary
1. Buy the correct licenses
1. Configure information barriers

## Step 1. Determine if information barriers are necessary

### Overview of Information Barriers

Information barriers are a great way to control who can communicate with one another in Microsoft Teams. Information barriers use Azure Active Directory (Azure AD) attributes to segment Azure AD users. The segmentation of users determines which users can talk to one another.

It's important to plan the segmentation of users. You can segment users based on what department they belong to, what Azure AD group they are a member of, or even by their usage location. A full list of attributes can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide#reference).

### Information Barrier Example

For example, you may choose to segment users based on the "Group" attribute. You want to allow users in the Azure AD Group "A" to communicate with users in the Azure AD Group "B", but not with the users in Azure AD Group "C". Information barriers can use the "Group" attribute to allow Group A to communicate with Group B but not with Group C.

>[!NOTE]
> To learn more about information barriers, see the following docs:
>
> - [Overview of information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide).
> - [Overview of segmentation and attributes](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide).

## Step 2. Buy the correct licenses

The following licenses are required:

- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis#who-uses-azure-ad)
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams

In order for information barriers to work, an information barrier license is required. The following licensing suites include information barrier licenses:

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

For more information, see [Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)

>[!NOTE]
> If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

## Step 3. Create Service Accounts

[Create a Service account](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)

## Step 4. Configure information barriers

Finally, you'll need to configure the information barriers. Visit [this article on information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide) for full instructions.
