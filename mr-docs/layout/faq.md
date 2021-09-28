---
author: StaceyLaw
description: Answers to common questions about using Microsoft Dynamics 365 Layout
ms.author: slaw
ms.date: 02/24/2020
ms.service: crm-online
ms.topic: article
title: Dynamics 365 Layout FAQ
ms.reviewer: v-brycho
---

# Dynamics 365 Layout FAQ

Here are answers to common questions about using [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)].

## Is Dynamics 365 Layout being discontinued as a separate application?

Yes. For more information, see [Announcing the transition of Dynamics 365 Layout](https://aka.ms/LayoutTransition).

## How can I tell which version I'm using?

To see the version number for [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)], go to **Settings** > **About**.

To see the version number for [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)], go to **Settings**, and then look in the **About** section.

## Do I need the Dynamics 365 Layout apps for both Microsoft HoloLens and Windows Mixed Reality immersive headsets?

No, you can use each app separately, though they do work together as well. If you want to copy 3D models or layouts from your PC to your [!include[pn-hololens](../includes/pn-hololens.md)] 
or to [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Mixed Reality, you’ll need the 
[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

## What are the technical requirements for running the Dynamics 365 Layout apps?

-   [!include[pn-hololens](../includes/pn-hololens.md)]: Your headset must be running the [Windows 10 April 2018
    Update](https://support.microsoft.com/help/12643). 

-   [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Mixed Reality: Your PC must be running the [Windows 10 April 2018
    Update](https://support.microsoft.com/help/4028685). You’ll also need
    [Windows Mixed Reality motion
    controllers](https://support.microsoft.com/help/4040517) to use the
    app with your immersive headset.

-   [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)]: Your PC must be running the [Windows 10 April 2018
    Update](https://support.microsoft.com/help/4028685).

[Learn more about device options and technical requirements.](requirements.md)

## Do I need an Azure Active Directory (Azure AD) account to use Dynamics 365 Layout?

Yes, if you’re the admin, you’ll need an [!include[pn-azure](../includes/pn-azure.md)] AD account to distribute the
apps, and users of [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] and the [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] will need an [!include[pn-azure](../includes/pn-azure.md)] AD account to
sign in to the apps.

## Can I use the HoloLens clicker with Dynamics 365 Layout?

You can use the [!include[pn-hololens](../includes/pn-hololens.md)] clicker with [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] but it has limited functionality. You can use the clicker to do menu selections and to scan a room, but you can't use it to manipulate objects.

## Do I need to be connected to Wi-Fi to use Dynamics 365 Layout?

[!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] requires users to be signed in with their Active Directory account to access the application. Users need to be connected to Wi-Fi the very first time the application is launched. After the first launch, they need to be connected to Wi-Fi once every 30 days so that the application can validate that the user has a valid Active Directory account for continued use of the application.

[Learn about [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] Wi-Fi requirements](https://docs.microsoft.com/dynamics365/mixed-reality/import-tool/import-tool#do-i-need-to-be-connected-to-wi-fi-to-use-dynamics-365-import-tool-preview).

## Can I change the unit of measure in Dynamics 365 Layout to metric?

Yes, you can choose between U.S. and metric units from **Settings** \>
**Measurements** \> **Unit of measure**.

## What languages is Dynamics 365 Layout available in?

[!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] is available for [!include[pn-hololens](../includes/pn-hololens.md)]2 in the following locales:

- US
- Canada (English and French)
- UK
- Australia
- Germany
- France
- China
- Japan
- Taiwan (no speech support)
- Hong Kong SAR (no speech support)

[!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)], the [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)], and the [!include[pn-visio](../includes/pn-visio.md)] Add-in for [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] are
available only in English for [!include[pn-hololens](../includes/pn-hololens.md)]1. Additionally, to install the add-in, you’ll need to
[set the display language for Microsoft Office to
English](https://support.office.com/article/add-an-editing-language-or-set-language-preferences-in-office-663d9d94-ca99-4a0d-973e-7c4a6b8a827d).

## Where is Dynamics 365 Layout available?

[!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] is available worldwide. [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] can be used with [!include[pn-hololens](../includes/pn-hololens.md)] or a Mixed Reality headset/motion controller and a [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Ultra PC.

[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] devices are available in the following markets (English only):

Austria, Australia, Belgium, Bulgaria, Canada, China, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary Iceland, Ireland, Italy, Japan, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Netherlands, New Zealand, Norway, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden, Switzerland, Turkey, United Kingdom, United States

## How do I import AutoCAD models?

You can prepare your 3D models yourself using third-party conversion and optimization tools. After converting and optimizing the models, you use the [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] to prepare them for mixed reality. [Learn more about Dynamics 365 Import Tool (Preview)](../import-tool/index.md).

Still need help? Try our [user forums](https://community.dynamics.com/365/layout).

### See also
[Overview of Dynamics 365 Layout](index.md)<br/>
[Device options and technical requirements](requirements.md)<br/>
[Deploy Dynamics 365 Layout](buy-and-deploy-layout.md)<br/>
[User guide](user-guide.md)<br/>
[How-to videos](videos.md)<br/>



[!INCLUDE[footer-include](../includes/footer-banner.md)]