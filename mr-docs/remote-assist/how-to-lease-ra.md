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

# How to provide Remote Assist licenses to external users

This document assumes that you have read our [Remote Assist advanced deployment scenarios](out-of-tenant-overview.md) document. 

Information barriers are a great way to control who can search and collaborate with one another when using Microsoft Teams and Remote Assist. Specifically, information barrier policies determine and prevent the following kinds of unauthorized communications:

- Searching for a user
- Adding a member to a team
- Starting a chat session with someone
- Starting a group chat
- Inviting someone to join a meeting
- Sharing a screen
- Placing a call

Additional information about information barriers can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#what-happens-with-information-barriers).

In this article, we'll take a look at how to deploy Remote Assist licenses for users who are outside your tenant but still in your company. 

## Step 1. Determine if information barriers are necessary

### Overview of information barriers

Information barriers are a great way to control who can search and collaborate with one another when using Microsoft Teams and Remote Assist. Information barriers use Azure Active Directory (Azure AD) attributes to segment Azure AD users. The segmentation of users determines which users can talk to one another.

It's important to plan how you segment users. You can segment users based on different attributes, such as what department they belong to, what Azure AD group they are a member of, or even by their usage location. A full list of attributes can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide#reference). To see how an organization might approach defining segments and policies, consider the following [example](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide#example-contosos-departments-segments-and-policies). A downloadable Excel workbook is available to help you plan and define your segments and policies (and create your PowerShell cmdlets). [Get the workbook.](https://github.com/MicrosoftDocs/OfficeDocs-O365SecComp/raw/public/SecurityCompliance/media/InfoBarriers-PowerShellGenerator.xlsx)

### Information barriers key concepts

When you define policies for information barriers, you'll work with user account attributes, segments, "block" and/or "allow" policies, and policy application.

User account attributes are defined in Azure Active Directory (or Exchange Online). These attributes can include department, job title, location, team name, and other job profile details.

Segments are sets of users that are defined in the Office 365 Security & Compliance Center using a selected user account attribute. (See the list of supported attributes.)

Information barrier policies determine communication limits or restrictions. When you define information barrier policies, you choose from two kinds of policies:

"Block" policies prevent one segment from communicating with another segment.
"Allow" policies allow one segment to communicate with only certain other segments.
Policy application is done after all information barrier policies are defined, and you are ready to apply them in your organization.

Additional information about information barriers can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#what-happens-with-information-barriers).

### Information barrier example

Company ABC wants Company ABC support engineers to use Teams and vendors at vendor companies V1, V2, and V3 to use Remote Assist. Company ABC must create a service account for each vendor in V1, V2, and V3 and assign a Remote Assist license to each service account. By default, Company ABC experts and all service account users in V1, V2, and V3 can search and call each other. Company ABC wants to use information barriers to limit V1 to only searching and collaborating with the Company ABC support engineers assigned to collaborate with V1, and same for V2 and V3.

Company ABC decides to segment users based on the "Group" attribute:
* Remote Assist users in V1 are in Group "V1_RemoteAssistUser"
* Teams users who collaborate with V1 are in Group "V1_SupportEngineer"
* Remote Assist users in V2 are in Group "V2_RemoteAssistUser"
* Teams users who collaborate with V2 are in Group "V2_SupportEngineer"
* Remote Assist users in V3 are in Group "V3_RemoteAssistUser"
* Teams users who collaborate with V3 are in Group "V3_SupportEngineer"
 
Then, Company ABC sets up bi-directional searching and collaborating between:
* "V1_RemoteAssistUser" and "V1_SupportEngineer"
* "V2_RemoteAssistUser" and "V2_SupportEngineer"
* "V3_RemoteAssistUser" and "V3_SupportEngineer"

>[!NOTE]
> Infomation barriers enable bidirectional searching and collaborating, not unidirectional searching and collaborating.

>[!NOTE]
> To learn more about information barriers, see the following docs:
>
> - [Overview of information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide).
> - [Overview of segmentation and attributes](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide).


## Step 2. Buy the correct licenses

The following licenses are required to enable a service account user to use Remote Assist.

- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis#who-uses-azure-ad)
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams

If you would like to control who the service account user can search and collaborate with, you will need to assign the service account a information barrier license. The following licensing suites include information barrier licenses:

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

For more information, see [Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)

>[!NOTE]
> If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

## Step 3. Create service accounts

Learn how to use Azure AD to [create service accounts](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory).

## Step 4. Assign licenses

Learn how to [assign licenses](https://docs.microsoft.com/azure/active-directory/fundamentals/license-users-groups) to each service account user. 

## Step 5. Configure information barriers

Finally, you'll need to [configure the information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide).
