---
author: prashantyvr
description: Learn about the device, licensing, and other requirements for installing and using Microsoft Dynamics 365 Guides.
ms.author: prashan
ms.date: 03/12/2024
ms.topic: article
title: Device, licensing, and other requirements for Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Device, licensing, and other requirements for Dynamics 365 Guides

Review the requirements for Dynamics 365 Guides.

## Supported geographies and languages

Determine if Dynamics 365 Guides is available in your country or region and your language.

- For country or region, see [Geographical availability for Power Apps](https://dynamics.microsoft.com/availability-reports/georeport/) and filter the view by **Dynamics 365** > **Operations Apps**. Then scroll the table to see Dynamics 365 Guides availability.
- For language, see [Product availability by language](https://dynamics.microsoft.com/en-us/availability-reports/languagereport/). Dynamics 365 Guides is listed in the hierarchy under **Dynamics 365**>**Operations Apps**.

## Device requirements

The following table lists technical requirements for deploying and using Dynamics 365 Guides throughout your organization.

| Device | Platform | Operating system requirements | Details |
|---|---|---|---|
| Microsoft HoloLens | x86, ARM | Build 10.0.17763 or later.<p>HoloLens build 10.0.17134 is the earliest build that supports Dynamics 365 Guides. We recommend that you update HoloLens to newer versions when they become available.</p> | For information about how to use Windows Update for Business, Mobile Device Management, and Windows Server Update Services (WSUS), see [Manage updates to HoloLens](/HoloLens/hololens-updates).<p>**Note:** HoloLens includes the Microsoft Edge browser. You can't use Internet Explorer with HoloLens.</p> |
| A computer (PC) that is running Windows 10 (required to create guides) | x64 | A PC that runs Windows 10 with build 10.0.17763 (October 2018 Update 1809) or later.<br><br>**Minimum resolution**. Dynamics 365 Guides supports a minimum effective resolution of 800 x 600 pixels before information loss.  | A PC that runs Windows 10 is used to create and edit guides that will then be available on HoloLens. |

> [!TIP]
> [You can set up a device license for multiple operators on a shared HoloLens device](device-license.md). 

## Requirements for services, apps, and features

Review the product requirements for services, apps, and features related to Dynamics 365 Guides.

| Service, app, or feature | Product required| Learn more |
|---|---|---|
|Purchase a Dynamics 365 Field Service or Guides subscription and assign licenses|Microsoft Entra account<br><br>You'll need an Microsoft Entra account for each licensed user so they can sign in to the app.</li></ul> | [Get started with Microsoft Entra ID](/azure/active-directory/fundamentals/active-directory-whatis) |
|PC authoring app and HoloLens app| Dynamics 365 Guides| [Buy and deploy Dynamics 365 Guides](setup.md) |
|Microsoft Dataverse and Power Apps service|Dynamics 365 Guides (included with subscription)|[Buy and deploy Dynamics 365 Guides](setup.md) |
|Outbound calling/Teams collaboration from Dynamics 365 Guides| Microsoft Teams or Dynamics 365 Remote Assist<br><br>A Microsoft Teams license *is not* included with a Dynamics 365 Guides license. A Microsoft Teams license *is* included with a Dynamics 365 Remote Assist license.</p> | [Learn more about calling from Dynamics 365 Guides](calling-start-call.md) |
|Analytics dashboard| Power BI Desktop app ([available as a free download](https://powerbi.microsoft.com/desktop/)).</p> | [Learn more about Power BI](https://powerbi.microsoft.com/desktop/) |
|Access your calendar and see scheduled meetings to join | [Exchange Online](https://www.microsoft.com/en-us/microsoft-365/business/compare-all-microsoft-365-business-products-b) |[Learn more about Exchange Online](/exchange/exchange-online) |
|Access and share OneDrive for Business files | [OneDrive for Business](https://www.microsoft.com/en-us/microsoft-365/onedrive/compare-onedrive-plans) |[Learn more about OneDrive](/sharepoint/onedrive-overview) |

## Calling features

You must have a Microsoft Teams license to use the calling features in Dynamics 365 Guides. This section describes specific Microsoft Teams requirements and describes limitations for calling features.

Dynamics 365 Guides supports new Teams seamlessly. No migration required. Learn more: [New Microsoft Teams app](https://adoption.microsoft.com/en-us/new-microsoft-teams/).

### Microsoft Teams requirements

| Device                             | OS requirement                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Microsoft Teams app on Windows 10 (or later) PC | Any Windows 10 (or later) build  | A Windows 10 PC running the Teams PC application can collaborate with a Dynamics 365 Guides user on HoloLens 2. |
| Microsoft Teams app on a mobile device | Any iOS or Android phone or tablet running  Microsoft Teams | A phone or tablet running the Microsoft Teams mobile app can collaborate with a Dynamics 365 Guides user on HoloLens 2.|

The Microsoft Teams user can be in the same organization as the Dynamics 365 Guides user, in a federated organization, or a guest in the organization.

### Limitations

Dynamics 365 Guides does not support:

- [Creating and managing assets](/dynamics365/mixed-reality/remote-assist/asset-capture-overview) either within or outside a Dynamics 365 Guides call.
- Creating and sharing one-time-call links.

## Next steps

- [Setup overview](setup.md)
- [Set up a device license for multiple operators on a shared HoloLens device](device-license.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
