---
author: prashantyvr
description: Answers to common questions about deploying Microsoft Dynamics 365 Remote Assist.
ms.author: prashan
ms.date: 06/07/2024
ms.topic: article
title: Frequently asked questions for deploying Dynamics 365 Remote Assist 
ms.reviewer: v-wendysmith
---

# Frequently asked questions for deploying Dynamics 365 Remote Assist

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

Here are some answers to common questions about deploying Dynamics 365 Remote Assist on HoloLens, HoloLens 2, and mobile devices.

## Which Microsoft platforms is Dynamics 365 Remote Assist dependent on?
 
Dynamics 365 Remote Assist is dependent on three Microsoft platforms:
 
- Microsoft Dataverse
- Microsoft Dynamics 365 Core Service
- Microsoft Teams
 
In rare cases, changes to these underlying platforms can cause issues in Dynamics 365 Remote Assist. Likewise, a change to one of these platforms can resolve a Dynamics 365 Remote Assist issue. To learn about the schedule for changes to these platforms, see the following topics:

- [Released versions of Microsoft Dataverse](/dynamics365/released-versions/microsoft-dataverse)
- [Released versions of Dynamics 365 Core Service Scheduling](/dynamics365/released-versions/dynamics365-css)
- [Update history for Microsoft Teams app version (Public Cloud and GCC)](/officeupdates/teams-app-versioning)

## When do I need to update the Dynamics 365 Remote Assist model-driven app (Remote Assist solution)?

You don't need to use the [Dynamics 365 Remote Assist model-driven app](ra-webapp-install.md) to empower technicians to collaborate efficiently from different locations on HoloLens, Android, or iOS devices. By installing the model-driven app, users gain access to additional functionality, however. 

If your organization uses any of the following features, you'll need to update the model-driven app when there are enhancements or bug fixes associated with these features: 

- [Capture and view asset data](asset-capture-overview.md)
- [Create and share one-time call links](one-time-call.md) 
- [Monitor operational metrics through the Calls Dashboard](calls-dashboard.md) 

Enhancements and bug fixes associated with these features are recorded in [What's new in Dynamics 365 Remote Assist](whats-new.md).

[Learn how to update the model-driven app](ra-webapp-install.md#update-the-model-driven-app-to-the-latest-version)

## Does Dynamics 365 Remote Assist mobile support conditional access policies?

Dynamics 365 Remote Assist mobile supports Azure Conditional Access policies through Microsoft Intune mobile application management (MAM). If a Conditional Access policy restricts file sharing for iOS devices, an error appears when the user selects the **Attach file** button in Dynamics 365 Remote Assist mobile, and then the **Attach file** button disappears. On Android, files will not upload when the restriction policy is set. Your organization may have older ["classic" Conditional Access policies](/azure/active-directory/conditional-access/policy-migration) that require managed apps, but Dynamics 365 Remote Assist mobile does not support classic Conditional Access policies. To work around this issue, replicate the classic policy as a new Conditional Access policy, and then delete the classic policy. [Learn more](/azure/active-directory/conditional-access/policy-migration).  

> [!NOTE]
> Conditional Access policies do not apply to Dynamics 365 Remote Assist on HoloLens.

## Can I use Dynamics 365 Remote Assist to collaborate with a Microsoft Teams user outside my tenant, or vice versa?

Yes. Learn how to [set up multi-tenant company deployments](multi-tenant-deployment.md), [enable vendors and contractors to use Remote Assist](vendor-use-ra.md), or [enable vendors and contractors to use Teams](vendor-use-teams.md).

## How do I set up Dynamics 365 Field Service to work with Dynamics 365 Remote Assist?

To learn how to set up Dynamics 365 Field Service integration with Dynamics 365 Remote Assist so that a firstline worker can call an expert in the context of a Field Service booking, see [Integrate Dynamics 365 Field Service with Dynamics 365 Remote Assist](troubleshoot-field-service.md).

## Will any Teams license work when communicating with a Dynamics 365 Remote Assist user?

Yes. Anyone that can sign in and use the Teams application on a Windows 10 PC or mobile device can communicate with a Dynamics 365 Remote Assist user if their tenants are set up correctly. If the Teams user and Dynamics 365 Remote Assist user are not in the same tenant, learn how to [set up multi-tenant company deployments](multi-tenant-deployment.md), [enable vendors and contractors to use Dynamics 365 Remote Assist](vendor-use-ra.md), or [enable vendors and contractors to use Teams](vendor-use-teams.md). 

## Can I assign a Dynamics 365 Remote Assist license to a user using [Microsoft Entra B2B](/azure/active-directory/b2b/what-is-b2b)?

No.  Dynamics 365 Remote Assist licenses must be assigned to a Microsoft Entra account created in the tenant where Dynamics 365 Remote Assist will be used.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
