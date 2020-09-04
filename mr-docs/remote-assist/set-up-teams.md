---
author: sophiasysun
description: Set up Microsoft Teams with Dynamics 365 Remote Assist 
ms.author: sopsun
ms.date: 04/07/2020
ms.service: crm-online
ms.topic: article
title: Set up Microsoft Teams with Dynamics 365 Remote Assist 
ms.reviewer: krbjoran
---

# Set up Microsoft Teams with Dynamics 365 Remote Assist  

A technician or inspector can use Dynamics 365 Remote Assist to work collaboratively with a remote colleague (typically an expert in a particular field) who uses Microsoft Teams. 

## Prerequisites

Learn about the licensing and device requirements [here](requirements.md).

## How to set up Teams depending on your scenario

Dynamics 365 Remote Assist users and Teams users may be in the same tenant or different tenants. How you set up Teams depends on your scenario.

| Scenario                                                                                                                                                                                                                                                                                                                    | Teams set up required                                                                                                                                                                          |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| People who want to use Dynamics 365 Remote Assist and people who want to use Teams are both currently in your tenant                                                                                                                                                                                                                | [Assign Teams licenses to people in your tenant](https://docs.microsoft.com/MicrosoftTeams/user-access).                                                             |
| Advanced deployment: [Multi-tenant company deployment using federation](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-1-federation) | The administrator of the tenant with users who want to use Teams must [assign Teams licenses to people in their tenant](https://docs.microsoft.com/MicrosoftTeams/user-access).                      |
| Advanced deployment: [Multi-tenant company deployment using guesting](https://docs.microsoft.com/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-2-guesting)      | The administrator of the tenant with Dynamics 365 Remote Assist users must [use Teams guesting](https://docs.microsoft.com/microsoftteams/guest-access-checklist) to enable people outside their tenant to use Teams.  |
| Advanced deployment: [Vendors and contractors are outside your tenant and want to use Dynamics 365 Remote Assist](vendor-use-ra.md)                                                                                                                                                                                                                                        | [Assign Teams licenses to people in your tenant](https://docs.microsoft.com/MicrosoftTeams/user-access).                                                             |

Need more help? Check out [Dynamics 365 Remote Assist FAQs](faq-deploy.md) for answers to common questions, or check out the [Microsoft Teams admin documentation](https://docs.microsoft.com/microsoftteams).
