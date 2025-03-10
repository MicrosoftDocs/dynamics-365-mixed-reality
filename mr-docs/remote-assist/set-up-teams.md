---
author: prashantyvr
description: Set up Microsoft Teams so a Dynamics 365 Remote Assist worker can work collaboratively. 
ms.author: prashan
ms.date: 06/07/2024
ms.topic: how-to
title: Set up Microsoft Teams for Dynamics 365 Remote Assist 
ms.reviewer: v-wendysmith
---

# Set up Microsoft Teams with Dynamics 365 Remote Assist  

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

A technician or inspector can use Remote Assist to work collaboratively with a remote colleague (typically an expert in a particular field) who uses Microsoft Teams. The remote collaborator might only want to [join a Remote Assist call on a one-time basis](common-deployment-scenarios.md#scenario-3-vendors-and-customers-join-one-time-call). Or, they might want to collaborate with a Remote Assist user long-term.  

This document explains the deployment required for different scenarios.

## Enable someone to join a Remote Assist call on a one-time basis using the Teams desktop app 

The licensed Remote Assist user can [set up a Teams meeting](./join-meeting-hololens.md) and invite the collaborator. Then, the licensed Remote Assist HoloLens user [joins the meeting using the Remote Assist HoloLens app](join-meeting-hololens.md). The Teams desktop user sees the meeting invitation in their Outlook calendar or Teams calendar. They right-click the meeting invitation and select **Join Teams meeting**. The web browser might launch and display options for joining the meeting. To join via Teams application, select **Launch it now**.

> [!Note] 
> Only a Remote Assist user and Teams desktop users can join a meeting. Remote Assist mobile users and Teams mobile users cannot join a meeting.

## Enable someone to make calls to and receive calls from a Remote Assist user long-term

| Scenario                                                                                                                                                                                                                                                                                                                    | How to enable someone to use Teams desktop app or Teams mobile app                                                                                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| People who want to use Dynamics 365 Remote Assist and people who want to use Teams are both currently in your tenant                                                                                                                                                                                                                | [Assign Teams licenses to people in your tenant](/MicrosoftTeams/user-access).                                                             |
| Advanced deployment: [Multitenant company deployment using federation](./multi-tenant-deployment.md) | The administrator of the tenant with users who want to use Teams must [assign Teams licenses to people in their tenant](/MicrosoftTeams/user-access).                      |
| Advanced deployment: [Multitenant company deployment using guest access](./multi-tenant-deployment.md)      | The administrator of the tenant with Dynamics 365 Remote Assist users must [use Teams guest access](/microsoftteams/guest-access-checklist) to enable people outside their tenant to use Teams.  |
| Advanced deployment: [Vendors and contractors are outside your tenant and want to use Dynamics 365 Remote Assist](vendor-use-ra.md)                                                                                                                                                                                                                                        | [Assign Teams licenses to people in your tenant](/MicrosoftTeams/user-access).                                                             |

Need more help? Check out [Dynamics 365 Remote Assist FAQs](faq-deploy.md) for answers to common questions, or check out the [Microsoft Teams admin documentation](/microsoftteams).


[!INCLUDE[footer-include](../includes/footer-banner.md)]
