---
author: sophiasysun
description: Vendor and contractor usage of Remote Assist
ms.author: sopsun
ms.date: 04/02/2020
ms.service: crm-online
ms.topic: article
title: Vendor and contractor usage of Remote Assist
ms.reviewer: krbjoran
---

# Vendor and contractor usage of Remote Assist

A Remote Assist call involves one party (technician) using Remote Assist and the other using Teams (expert or remote collaborator).  In most cases, technicians and remote collaborators all belong to the same tenant, and thus a [standard deployment of Remote Assist](deploy-remote-assist.md) and [standard deployment of Teams](set-up-teams.md) is all you need. 

However, there are certain scenarios where this may not be the case: 

1. **Multi-tenant company deployments**: A company has multiple organizations or business units, each with their own tenant, that want to collaborate using Remote Assist. Or, multiple companies want to collaborate using Remote Assist. Users who want to use Remote Assist already have Remote Assist licenses, and users who want to use Teams already have Teams licenses. Learn more about multi-tenant collaboration in this document. [Learn more about this scenario.](multi-tenant-deployment.md) 

2. **Vendors and contractors use Remote Assist app**: A company wants vendors and contractors who do not already have Remote Assist and aren’t part of the company tenant to use Remote Assist. [Learn more about this scenario.](vendor-use-ra.md) 

3. **Vendors and contractors use Teams app**: A company wants employees to use Remote Assist HoloLens to receive assistance from out-of-tenant collaborators without needing to set up guest access or external access. This document focuses on this scenario.

## Scenario overview

Companies may want to receive assistance from non-company collaborators. However, companies do not want to set up guest access or external access with the non-company collaborators' tenant (sometimes, the collaborator may not be part of an AAD tenant.) 

## Example

Company ABC purchased equipment from an OEM and has HoloLenses. Company ABC  wants a quick and easy way to enable an expert from the OEM to join the call and guide a Company ABC employee to set up the equipment. Company ABC does not want to have to set up guest access (i.e. enable guest access for Company ABC tenant and guest the expert into a specific Teams team) or external access with the OEM's tenant. Company ABC employee knows the expert's email, and wants to invite the expert to join a Remote Assist call.

## Implementation

The Remote Assist HoloLens user from Company ABC will set up a meeting and invite the out-of-tenant collaborator via email. Then, the Remote Assist HoloLens user will join the meeting from the Remote Assist HoloLens app.

[!Note] Only a Remote Assist user and Teams desktop user(s) can join a meeting. Remote Assist mobile users and Teams mobile users cannot join a meeting.


## Prerequisite

Prerequisites for tenant: 
1.	[Allow anonymous users to join meetings](https://docs.microsoft.com/en-us/microsoftteams/meeting-settings-in-teams#allow-anonymous-users-to-join-meetings)
2.	See [additional meeting settings](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) a tenant can configure, including requiring a meeting organizer to let anonymous users into a call from the lobby 

Prerequisites for the Remote Assist HoloLens user (who will join the call as an authenticated RA user)
1. D365 Remote Assist is installed on the HoloLens
2. Has 

Prerequisites for the Teams Desktop user (who will join the call as an anonymous Teams user)
1. Teams desktop application is downloaded. No licenses needed.  
2. Access to email  

## Steps

1.	Remote Assist HoloLens user schedules the meeting using Outlook or Teams (mobile or desktop) and invites the out-of-tenant user by using their preferred email address.
a.	If scheduling using Outlook, ensure the "Teams Meeting" option is enabled. Send.
2.	RA HL user logs into RA on HL with the account used to schedule the meeting.
3.	RA HL user views “Join Meeting” under the Recent Contacts panel, and selects “Join Meeting” 
4.	Teams desktop user views email invitation and selects “Join Teams Meeting" link in the email invite.
a.	A Web instance will launch and display options for joining the meeting (see screenshot). Teams desktop user will have an option to join via Web or by via Teams application. Click the small text link "Launch it now.”
 
b.	Enable video and/or audio and indicate name
c.	Join meeting 
5.	Now, the Teams desktop user can view the HL user’s video feed and both can annotate. 

Notes:
1.	This will not work if the RA HL user tries to create a meeting using the Teams “Meet Now” feature 
2.	Teams desktop experience limitations
1.	I believe that as an anonymous participant, the Teams desktop user will not be able to share files from OneDrive, but they may be able to “display” files in the RA HL environment via screen share.
2.	Teams desktop user cannot add additional people to the call. Only the RA HL user can, by sharing the link with additional people.
3.	RA HL experience limitations 
1.	RA HL user can't create the meeting from within the Remote Assist app.
2.	RA HL user cannot use RA to let anonymous participants into the call from the lobby. The RA HL user may have to use Teams to do so. 
 





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

You can segment users based on different attributes, such as what department they belong to, what Azure AD group they are a member of, or even by their usage location. A full list of attributes can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide#reference). To see how an organization might approach defining segments and policies, consider the following [example](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide#example-contosos-departments-segments-and-policies). A downloadable Excel workbook is available to help you plan and define your segments and policies (and create your PowerShell cmdlets). [Download the workbook (xlsx file).](https://github.com/MicrosoftDocs/OfficeDocs-O365SecComp/raw/public/SecurityCompliance/media/InfoBarriers-PowerShellGenerator.xlsx). Additional information about information barriers can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide).

3. Buy the correct licenses

Learn about [licenses required to use Remote Assist](requirements.md).

If you would like to control who the service account user can search and collaborate with, you will need to assign the service account an information barrier license. The following licensing suites include information barrier licenses:

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

For more information, see [Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)

4. [Create service accounts](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory).

5. [Assign licenses](https://docs.microsoft.com/azure/active-directory/fundamentals/license-users-groups) to each service account user. 

6. If information barriers are necessary, [configure information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide).



