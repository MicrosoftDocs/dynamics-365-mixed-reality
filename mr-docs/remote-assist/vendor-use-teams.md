---
author: sophiasysun
description: Vendors and contractors use Microsoft Teams 
ms.author: sopsun
ms.date: 05/06/2020
ms.service: crm-online
ms.topic: article
title: Vendors and contractors use Microsoft Teams 
ms.reviewer: krbjoran
---

# Vendors and contractors use Microsoft Teams

A Dynamics 365 Remote Assist call involves one party (for example, technician) using Dynamics 365 Remote Assist and the other using Teams (for example, expert or remote collaborator). In most cases, technicians and remote collaborators all belong to the same tenant, so a [standard deployment of Dynamics 365 Remote Assist](deploy-remote-assist.md) and [standard deployment of Teams](set-up-teams.md) is all you need. 

However, there are some scenarios where this may not be the case.

1. **Multi-tenant company deployments**: A company has multiple organizations or business units (each with their own tenant) that want to collaborate using Dynamics 365 Remote Assist. Or, multiple companies want to collaborate using Dynamics 365 Remote Assist. Users who want to use Dynamics 365 Remote Assist already have Dynamics 365 Remote Assist licenses, and users who want to use Teams already have Teams licenses. They want to initiate unplanned calls and meetings with each other. [Learn more about this scenario.](multi-tenant-deployment.md) 

2. **Vendors and contractors use Dynamics 365 Remote Assist app**: A company wants vendors and contractors who do not already have Dynamics 365 Remote Assist and aren’t part of the company tenant to use Dynamics 365 Remote Assist. [Learn more about this scenario.](vendor-use-ra.md) 

3. **Vendors and contractors use Teams app**: A company wants to provide employees with a quick and easy way to use Dynamics 365 Remote Assist HoloLens to receive assistance from out-of-tenant collaborators who may or may not have Teams. The company does not want to set up guest access or external access. This document focuses on this scenario.

## Scenario overview

A company wants to provide employees with a quick and easy way to use Dynamics 365 Remote Assist HoloLens to receive assistance from out-of-tenant collaborators who may or may not have Teams. The company does not want to set up guest access or external access.

Let's consider the following example.

Company ABC purchased equipment from an OEM. An ABC employee has trouble setting up the equipment, and wants an easy way for an expert from the OEM to join the call and provide remote assistance via mixed reality annotations. The ABC employee knows the expert's email and wants the expert to join the Dynamics 365 Remote Assist call using Teams desktop - even if they don't have a Teams license.

## Prerequisites

**Prerequisite for Company ABC tenant:**
1.	[Allow anonymous users to join meetings](/microsoftteams/meeting-settings-in-teams#allow-anonymous-users-to-join-meetings).

**Prerequisites for the Company ABC employee who will use Dynamics 365 Remote Assist HoloLens:**
1. Dynamics 365 Dynamics 365 Remote Assist app is installed on the HoloLens.
2. Employee has the out-of-tenant collaborator's email address.

**Prerequisites for the out-of-tenant collaborator who will use Teams desktop:**
1. Teams desktop app is downloaded. (Teams license not needed).
2. Access to email.

## Steps

The Dynamics 365 Remote Assist HoloLens user from Company ABC will set up a meeting and invite the out-of-tenant collaborator via email. Then, the Dynamics 365 Remote Assist HoloLens user will join the meeting from the Dynamics 365 Remote Assist HoloLens app. The out-of-tenant collaborator will join the meeting from the Teams desktop app.

> [!Note]
> Only a Dynamics 365 Remote Assist user and Teams desktop users can join a meeting. Dynamics 365 Remote Assist mobile users and Teams mobile users cannot join a meeting.

1. Dynamics 365 Remote Assist HoloLens user schedules the meeting using [Outlook](https://support.office.com/article/Schedule-a-meeting-with-other-people-5C9877BC-AB91-4A7C-99FB-B0B68D7EA94F) or [Teams](https://support.office.com/article/Schedule-a-meeting-in-Teams-943507a9-8583-4c58-b5d2-8ec8265e04e5) (mobile or desktop) and invites the out-of-tenant user by using their preferred email address. 
2. Dynamics 365 Remote Assist HoloLens user logs into Dynamics 365 Remote Assist with the account used to schedule the meeting.
3. Dynamics 365 Remote Assist HoloLens user sees **Join Meeting** under the **Recent Contacts** panel, and selects **Join Meeting**. 
4. Teams desktop user sees the meeting invitation in their Outlook calendar or Teams calendar. They right-click the meeting invitation and select **Join Teams meeting**. (The web browser may launch and display options for joining the meeting. To join via Teams application, select **Launch it now**.)
5. Teams desktop user indicates name and joins meeting.
6. Now, the Teams desktop user can view the Dynamics 365 Remote Assist HoloLens user’s video feed and both can annotate. 

## Additional notes

1. The steps outlined in this article won't work if the Dynamics 365 Remote Assist HoloLens user tries to create a meeting using the Teams **Meet Now** feature.
2. If Company ABC has not set up external access with the out-of-tenant collaborator's tenant, the collaborator will join the Dynamics 365 Remote Assist call as an anonymous Teams meeting participant. Anonymous Teams meeting participants experience some limitations. For example, the Teams desktop user can't share files from OneDrive, but they are able to display files in the Dynamics 365 Remote Assist HoloLens user's environment by sharing their screen. Furthermore, the Teams desktop user can't add additional people to the call; only the Dynamics 365 Remote Assist HoloLens user can. The Dynamics 365 Remote Assist HoloLens user can invite additional Teams desktop users to the call by sharing the Teams meeting link with them or by sending the meeting invite to them. (The Dynamics 365 Remote Assist HoloLens user won't be able to directly call out-of-tenant users into the Dynamics 365 Remote Assist call if external access or guest access with those users is not set up.)
3. Dynamics 365 Remote Assist HoloLens doesn't support letting anonymous participants into the call from the lobby.





[!INCLUDE[footer-include](../includes/footer-banner.md)]