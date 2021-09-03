---
author: Mamaylya
description: Learn about the device and licensing requirements for installing and using Microsoft Dynamics 365 Guides.
ms.author: mamaylya
ms.date: 12/09/2020
ms.topic: article
title: Device and licensing requirements for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Device and licensing requirements for Dynamics 365 Guides

The following table lists technical requirements for deploying and using [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] throughout your organization.

## Device requirements
| Device | Platform | Operating system requirements | Details |
|---|---|---|---|
| [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] | x86, ARM | Build 10.0.17134 or later.<p>[!include[pn-hololens](../includes/pn-hololens.md)] build 10.0.17134 is the earliest build that supports [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. We recommend that you update [!include[pn-hololens](../includes/pn-hololens.md)] to newer versions when they become available.</p> | For information about how to use [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Update for Business, Mobile Device Management, and [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Server Update Services (WSUS), see [Manage updates to HoloLens](/HoloLens/hololens-updates).<p>**Note:** HoloLens includes the Microsoft Edge browser. You can't use Internet Explorer with HoloLens.</p> |
| A computer (PC) that is running [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 (required to create guides) | x64 | A PC that runs [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 with build 10.0.17134 (April 2018 Update 1803) or later.<br><br>**Minimum resolution**. Dynamics 365 Guides supports a minimum effective resolution of 800 x 600 pixels before information loss.  | A PC that runs [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 is used to create and edit guides that will then be available on [!include[pn-hololens](../includes/pn-hololens.md)]. |

## Dynamics 365 Guides licensing and product requirements

| Product required | Details | Learn more |
|---|---|---|
| [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] | [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] software that is running on a PC and [!include[pn-hololens](../includes/pn-hololens.md)] that has a valid [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] subscription are required.<p>**Note:** Microsoft Dataverse and the Power Apps service are included with the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] subscription for individuals who use a [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] license.</p> | [Buy and deploy Dynamics 365 Guides](setup.md)<p>You can also [sign up for a free trial Dynamics 365 subscription](setup.md).</p> |
| Dynamics 365 Remote Assist </br> or Microsoft Teams | [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] requires these licenses to enable outbound calling from Dynamics 365 Guides.</p> | [Learn more about calling from Dynamics 365 Guides](https://powerbi.microsoft.com/desktop/) |
| [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop app | [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] requires the [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop app to view the Analytics dashboard.<p>**Note:** [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop is [available as a free download](https://powerbi.microsoft.com/desktop/).</p> | [Learn more about Power BI](https://powerbi.microsoft.com/desktop/) |
| Azure Active Directory (Azure AD) account | Required for:<ul><li>Purchasing [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] subscription and assigning licenses. You'll need an Azure AD account for each licensed user.</li><li>Users when signing in to the app.</li></ul> | [Get started with Azure AD](/azure/active-directory/fundamentals/active-directory-whatis) |
| Network connectivity | Internet access is required to download the app and use all its features for both PC and [!include[pn-hololens](../includes/pn-hololens.md)]. | |

## Device options and requirements for a Microsoft Teams user

| Device                             | OS requirements                                             | Details                                                                                                                                                                                                                                                                                 |
| ---------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Microsoft Teams app on Windows 10 PC | Any Windows 10 build.                                       | A Windows 10 PC running the Teams PC application can collaborate with a Dynamics 365 Guides user on HoloLens 2. |
| Microsoft Teams app on a mobile device | Any iOS or Android phone or tablet running  Microsoft Teams. | A phone or tablet running the Microsoft Teams mobile app can collaborate with a Dynamics 365 Guides user on HoloLens 2.|

> [!Note] 
> Dynamics 365 Guides might not be available in your country. For more information, see [Dynamics 365 Guides availability](./mobile-app/faq-mobile.md).

## Licensing and product requirements per role

### Dynamics 365 Guides on HoloLens - Calling

A licensed Dynamics 365 Guides HoloLens user can initiate calls to a Microsoft Teams user if the Dynamics 365 Guides users has licenses for either of the following products:

- Dynamics 365 Remote Assist
- Microsoft Teams

> [!NOTE]
> Dynamics 365 Remote Assist and Dynamics 365 Guides do not currently comply with Microsoft Teams policies. </br>
> Outbound calls from Dynamics 365 Guides are not included in Dynamics 365 Remote Assist call record analytics/insights.

| **Included with Dynamics 365 Guides license** | **What capabilities are available?**                                                                                                                                                                                                                                                                                                       |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Dynamics 365 Guides</br> and Microsoft Teams**             | Make outbound calls using the Dynamics 365 Guides app on HoloLens 2.|
| **Dynamics 365 Guides </br>and Dynamics 365 Remote Assist**             | Make outbound calls using the Dynamics 365 Guides app on HoloLens. <!--This should also be HoloLens 2, correct?-->|

An Azure Active Directory account is required to purchase a Dynamics 365 Remote Assist or Dynamics 365 Guides subscription and to assign licenses. You need an Azure AD account for each licensed user. They'll use this account when signing in to the app. 

> [!Note]
> The Dynamics 365 Remote Assist, Teams, and Dataverse licenses must be assigned to a native member of the tenant ([Azure AD member](/azure/active-directory/fundamentals/users-default-permissions#member-and-guest-users) account). Dynamics 365 Remote Assist does not support [Azure AD B2B](/azure/active-directory/external-identities/what-is-b2b); an individual cannot sign into Dynamics 365 Remote Assist using a Dynamics 365 Remote Assist license assigned to an Azure AD guest account. 

#### Limitations

The calling feature in Dynamics 365 Guides does not support:

- Access to the Dynamics 365 Remote Assist model-driven app.
- [Creating and managing assets](./asset-capture-overview.md) either within or outside a Dynamics 365 Guides call.
- Creating and sharing one-time-call links.
- Creating or viewing analytics and insights based on your call records. 

### Microsoft Teams app user - Receiving calls

| **License held by Microsoft Teams user**                                                                                     | **Capabilities in a Dynamics 365 Guides call**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| None                                                                                                                           | The Microsoft Teams desktop user can accept an inbound call from a Dynamics 365 Guides user.                                                                                                                                                                                                                                                                                          |
| Microsoft Teams                                                                                                                          | The Microsft Teams user’s experience is **_identical_** regardless of whether the Microsoft Teams user is: <!--And is it the same as the None case above? Can acceet inbound calls only--><br></br> - A member in the Dynamics 365 Guides user’s tenant </br> - [A guest](./multi-tenant-deployment.md#solution-2-guest-access) in the Dynamics 365 Guides user’s tenant </br> - A member in a tenant that’s [federated](./multi-tenant-deployment.md#solution-1-external-access-federation) with the Dynamics 365 Guides user’s tenant (Teams desktop only) </br><br> [Learn about exceptions to the above Microsoft Teams experience](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) </br>|



## What's next

[Setup overview](setup.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
