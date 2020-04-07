---
author: sophiasysun
description: Set up Microsoft Teams with Dynamics 365 Remote Assist 
ms.author: sopsun
ms.date: 03/15/2020
ms.service: crm-online
ms.topic: article
title: Set up Microsoft Teams with Dynamics 365 Remote Assist 
ms.reviewer: krbjoran
---

# Set up Microsoft Teams with Dynamics 365 Remote Assist  

A Remote Assist user can use mixed reality annotations to work collaboratively with a colleague (typically an expert in a particular field) who uses Microsoft Teams. The remote collaborator can see everything that the Remote Assist user sees, and they can draw and 
annotate together. 

Setting up this collaboration is simple.

## Prerequisites

Learn about the licensing and device requirements [here](requirements).

## How to set up Teams depending on your scenario

Remote Assist users and Teams users may be in the same tenant or different tenants. How you set up Teams depends on your scenario.

| Scenario                                                                                                                                                                                                                                                                                                                    | Teams set up required                                                                                                                                                                          |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| People who want to use Remote Assist and people who want to use Teams users are currently in the same tenant                                                                                                                                                                                                                | [Assign Teams license to people in your tenant](https://docs.microsoft.com/en-us/MicrosoftTeams/user-access) who want to use Teams                                                             |
| Advanced deployment: [Multi-tenant company deployment using federation]([https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-1-federation](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-1-federation)) | [Assign Teams license to people in your tenant](https://docs.microsoft.com/en-us/MicrosoftTeams/user-access) who want to use Teams                                                             |
| Advanced deployment: [Multi-tenant company deployment using guesting]([https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-2-guesting](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/remote-assist/multi-tenant-deployment#solution-2-guesting))       | [Use Teams guesting](https://docs.microsoft.com/en-us/microsoftteams/guest-access-checklist) to enable people outside your tenant to collaborate with you in specific Teams teams and channels |
| Advanced deployment: [Vendors and contractors use Remote Assist](vendor-use-ra.md)                                                                                                                                                                                                                                        | [Assign Teams license to people in your tenant](https://docs.microsoft.com/en-us/MicrosoftTeams/user-access) who want to use Teams                                                             |




Need more help? [Check out Dynamics 365 Remote Assist FAQs](faq.md) for answers to common questions, or check out the [Microsoft Teams admin documentation.](https://docs.microsoft.com/en-us/microsoftteams).
