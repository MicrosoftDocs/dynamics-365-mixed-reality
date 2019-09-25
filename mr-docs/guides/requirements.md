---
author: Mamaylya
description: Technical requirements for installing and using Dynamics 365 Guides
ms.author: mamaylya
ms.date: 10/01/2019
ms.service: crm-online
ms.topic: article
title: Technical requirements for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Requirements for Dynamics 365 Guides

The following table lists technical requirements for deploying and using [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] throughout your organization.

## Device requirements
|Device|OS requirements|Details|
|----------------------------------------|---------------------------------------------|-------------------------------------|
|[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)]|Build 10.0.17134 or later. HoloLens build 10.0.17134 is the minimum that supports Dynamics 365 Guides. We recommend updating HoloLens to newer versions when available. |See [Manage updates to HoloLens](https://docs.microsoft.com/en-us/HoloLens/hololens-updates) for instructions on using [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Update for Business, Mobile Device Management, and [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Server Update Services (WSUS).|
|[!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC (required to create a guide)|[!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC with build 10.0.17134 (April 2018 Update 1803) or later|A [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC is used to create and edit guides that will be then available on [!include[pn-hololens](../includes/pn-hololens.md)].|

## Licensing and product requirements

|Product required|Details|Learn more|
|-------------------------------|-------------------------------------------------------|-------------------------------------------|
|Dynamics 365 Guides|Dynamics 365 Guides software on PC and HoloLens with a valid Dynamics 365 Guides subscription is required.</br><br>**Note** The Common Data Service and PowerApps service are included with the Dynamics 365 Guides subscription for individuals using a Dynamics 365 Guides license.|[Buy and deploy Dynamics 365 Guides](setup.md)</br><br>You can also [sign up for a free trial Dynamics 365 subscription](setup.md).|
|Power BI desktop app|Dynamics 365 Guides requires the Power BI desktop app to view the Analytics dashboard.</br><br>**Note** Power BI desktop is [available as a free download](https://powerbi.microsoft.com/desktop/).|[Learn more about Power BI](https://powerbi.microsoft.com/desktop/)|
|Network connectivity|Internet access is required to download the app and to use all of its features for both PC and HoloLens.||
|Azure Active Directory (Azure AD) account|Required for:</br><br>- Purchasing Dynamics 365 Guides subscription and assigning licenses. You'll need an Azure AD account for each licensed user.</br><br>- Users when signing in to the app.|[Get started with Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis)|

### See also

[Buy and deploy Dynamics 365 Guides](setup.md)<br>
[Upgrade the solution (for admins)](upgrade.md)
