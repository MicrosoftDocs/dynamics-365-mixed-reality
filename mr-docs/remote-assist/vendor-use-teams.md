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

A Remote Assist call involves one party (e.g. technician) using Remote Assist and the other using Teams (e.g. expert or remote collaborator).  In most cases, technicians and remote collaborators all belong to the same tenant, and thus a [standard deployment of Remote Assist](deploy-remote-assist.md) and [standard deployment of Teams](set-up-teams.md) is all you need. 

However, there are certain scenarios where this may not be the case: 

1. **Multi-tenant company deployments**: A company has multiple organizations or business units, each with their own tenant, that want to collaborate using Remote Assist. Or, multiple companies want to collaborate using Remote Assist. Users who want to use Remote Assist already have Remote Assist licenses, and users who want to use Teams already have Teams licenses. They want to initiate ad hoc calls and meetings with each other. [Learn more about this scenario.](multi-tenant-deployment.md) 

2. **Vendors and contractors use Remote Assist app**: A company wants vendors and contractors who do not already have Remote Assist and aren’t part of the company tenant to use Remote Assist. [Learn more about this scenario.](vendor-use-ra.md) 

3. **Vendors and contractors use Teams app**: A company wants employees to use Remote Assist HoloLens to receive assistance from out-of-tenant collaborators without needing to set up guest access or external access. This document focuses on this scenario.

## Scenario overview

Companies may want to receive assistance from out-of-tenant collaborators without setting up guest access or external access with the collaborators' tenant (sometimes, the collaborator may not be part of an AAD tenant.) The Remote Assist HoloLens user from Company ABC will set up a meeting and invite the out-of-tenant collaborator via email. Then, the Remote Assist HoloLens user will join the meeting from the Remote Assist HoloLens app. The out-of-tenant collaborator will join the Remote Assist call via Teams desktop.

[!Note] Only a Remote Assist user and Teams desktop user(s) can join a meeting. Remote Assist mobile users and Teams mobile users cannot join a meeting.

## Example

Company ABC purchased equipment from an OEM and has HoloLenses. Company ABC  wants a quick and easy way to enable an expert from the OEM to join the call and guide a Company ABC employee to set up the equipment. Company ABC does not want to have to set up guest access (i.e. enable guest access for Company ABC tenant and guest the expert into a specific Teams team) or external access with the OEM's tenant. Company ABC employee knows the expert's email, and wants to invite the expert to join a Remote Assist call.

## Prerequisite

Prerequisites for tenant: 
1.	[Allow anonymous users to join meetings](https://docs.microsoft.com/en-us/microsoftteams/meeting-settings-in-teams#allow-anonymous-users-to-join-meetings)
2.	See [additional meeting settings](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) a tenant can configure, including requiring a meeting organizer to let anonymous users into a call from the lobby 

Prerequisites for the Remote Assist HoloLens user (who will join the call as an authenticated RA user)
1. D365 Remote Assist is installed on the HoloLens
2. Has the collaborator's email address

Prerequisites for the Teams Desktop user (who will join the call as an anonymous Teams user)
1. Teams desktop application is downloaded. No licenses needed.  
2. Access to email  

## Steps

1.	Remote Assist HoloLens user schedules the meeting using Outlook or Teams (mobile or desktop) and invites the out-of-tenant user by using their preferred email address.
 1. If scheduling using Outlook, ensure the "Teams Meeting" option is enabled. Send.
2.	Remote Assist HoloLens user logs into Remote Assist with the account used to schedule the meeting.
3.	Remote Assist HoloLens user views “Join Meeting” under the Recent Contacts panel, and selects “Join Meeting” 
4.	Teams desktop user views meeting invitation via Outlook calendar or Teams calendar. User right clicks the meeting invitation and selects "Join Teams meeting." A web instance may launch and display options for joining the meeting (see screenshot). To join via Teams application, the user should select "Launch it now." 
5. Teams desktop user indicates name and joins meeting
6.	Now, the Teams desktop user can view the HL user’s video feed and both can annotate. 

**Notes:**
1. This will not work if the Remote Assist HoloLens user tries to create a meeting using the Teams “Meet Now” feature 
2.	If Company ABC has not set up external access with the out-of-tenant collaborator's tenant, the collaborator will join the Remote Assist call as an anonymous Teams meeting participant. Anonymous Teams meeting participants experience some limitations. For example, the Teams desktop user cannot share files from OneDrive, but they are able to "display files" in the Remote Assist HoloLens user's environment by sharing their screen. Furthermore, the Teams desktop user cannot add additional people to the call - only the Remote Assist HoloLens user can. The Remote Assist HoloLens user can invite additional Teams desktop users to the call by sharing the Teams meeting link with them or by sending the meeting invite to them. (The Remote Assist HoloLens user will not be able to directly call out-of-tenant users into the Remote Assist call if external access or guest access with those users is not set up.)
3. Remote Assist HoloLens does not support letting anonymous participants in the call from the lobby.



