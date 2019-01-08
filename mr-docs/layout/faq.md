---
author: ornellaalt
description: Answers to common questions about using Microsoft Dynamics 365 Layout
ms.author: ornella
ms.date: 12/20/2018
ms.service: crm-online
ms.topic: article
title: Dynamics 365 Layout FAQ
ms.reviewer: v-brycho
---

# Dynamics 365 Layout FAQ

Here are answers to common questions about using [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)].

**How can I get [!include[pn-layout](../includes/pn-layout.md)]?**  

If you’re an IT admin, [learn how to try or buy, and deploy the app](../licensing/buy-and-deploy.md).  

**Can I try the app before buying it?**

Yes, [!include[pn-layout](../includes/pn-layout.md)] is available as a free 30-day trial. For more information, see [Try or buy,
and deploy Layout](../licensing/buy-and-deploy.md).

**Can I still use the preview app?**

The preview period has ended. Existing preview apps customers have until
December 31, 2018, to start a free trial of the General Availability app or to upgrade to a paid subscription.


**How can I tell which version I'm using?**

To see the version number for Layout, go to **Settings** > **About**.

To see the version number for the Import Tool, go to **Settings**, and then look in the **About** section.

**Do I need the Layout apps for both HoloLens and Windows Mixed Reality?**

No, you can use each app separately, though they do work together as well. If
you want to copy 3D models or layouts from your PC to your [!include[pn-hololens](../includes/pn-hololens.md)] or to
Windows Mixed Reality, you’ll need the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)].

**What are the technical requirements for running the [!include[pn-layout](../includes/pn-layout.md)] apps?**

-   [!include[pn-hololens](../includes/pn-hololens.md)]: Your headset must be running the [Windows 10 April 2018
    Update](https://support.microsoft.com/en-us/help/12643). 

-   [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Mixed Reality: Your PC must be running the [Windows 10 April 2018
    Update](https://support.microsoft.com/en-us/help/4028685). You’ll also need
    [Windows Mixed Reality motion
    controllers](https://support.microsoft.com/en-us/help/4040517) to use the
    app with your immersive headset.

-   [!include[pn-import-tool](../includes/pn-import-tool.md)]: Your PC must be running the [Windows 10 April 2018
    Update](https://support.microsoft.com/en-us/help/4028685).

[Learn more about device options and technical requirements.](requirements.md)

**Do I need an [!include[pn-azure-active-directory](../includes/pn-azure-active-directory.md)] ([!include[pn-azure](../includes/pn-azure.md)] AD) account to use [!include[pn-layout](../includes/pn-layout.md)]?**

Yes, if you’re the admin, you’ll need an [!include[pn-azure](../includes/pn-azure.md)] AD account to distribute the
apps, and users of [!include[pn-layout](../includes/pn-layout.md)] and the [!include[pn-import-tool](../includes/pn-import-tool.md)] will need an [!include[pn-azure](../includes/pn-azure.md)] AD account to
sign in to the apps.

**How often is [!include[pn-layout](../includes/pn-layout.md)] updated?**

[!include[pn-layout](../includes/pn-layout.md)] follows the Modern Lifecyle Policy with continuous service updates and major updates every 6 months (October/April). 


**Can I use the [!include[pn-hololens](../includes/pn-hololens.md)] clicker with [!include[pn-layout](../includes/pn-layout.md)]?**

You can use the [!include[pn-hololens](../includes/pn-hololens.md)] clicker with [!include[pn-layout](../includes/pn-layout.md)] but it has limited functionality. You can use the clicker to do menu selections and to scan a room, but you can't use it to manipulate objects.

**Do I need to be connected to Wi-Fi to use [!include[pn-layout](../includes/pn-layout.md)]?**

If you want to convert 3D models using the [!include[pn-import-tool](../includes/pn-import-tool.md)], you’ll need a Wi-Fi
connection if you use the cloud service option. If you choose to convert files
using the PC option, you don’t need a Wi-Fi connection.

**Can I change the unit of measure in the [!include[pn-layout](../includes/pn-layout.md)] app to metric?**

Yes, you can choose between U.S. and metric units from **Settings** \>
**Measurements** \> **Unit of measure**.

**What languages is [!include[pn-layout](../includes/pn-layout.md)] available in?**

At this time, [!include[pn-layout](../includes/pn-layout.md)], the [!include[pn-import-tool](../includes/pn-import-tool.md)], and the [!include[pn-visio](../includes/pn-visio.md)] Add-in for [!include[pn-layout](../includes/pn-layout.md)] are
available only in English. Additionally, to install the Add-in, you’ll need to
[set the display language for Microsoft Office to
English](https://support.office.com/article/add-an-editing-language-or-set-language-preferences-in-office-663d9d94-ca99-4a0d-973e-7c4a6b8a827d).

**Where is [!include[pn-layout](../includes/pn-layout.md)] available?**

[!include[pn-layout](../includes/pn-layout.md)] is available worldwide. [!include[pn-layout](../includes/pn-layout.md)] can be used with [!include[pn-hololens](../includes/pn-hololens.md)] or a Mixed Reality headset/motion controller and a [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Ultra PC.

[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] devices are available in the following markets (English only):

Austria, Australia, Belgium, Bulgaria, Canada, China, Croatia, Cyprus, Czech Republic, Denmark, Estonia, Finland, France, Germany, Greece, Hungary Iceland, Ireland, Italy, Japan, Latvia, Liechtenstein, Lithuania, Luxembourg, Malta, Netherlands, New Zealand, Norway, Poland, Portugal, Romania, Slovakia, Slovenia, Spain, Sweden, Switzerland, Turkey, United Kingdom, United States

**How does the [!include[pn-import-tool](../includes/pn-import-tool.md)] process my 3D models?**

There are three options for preparing 3D models for HoloLens or Mixed Reality headsets. You can use the [!include[cc-microsoft](../includes/cc-microsoft.md)] Cloud Service, your PC, or you can convert your models without optimizing them. [Learn more.](user-guide.md#file-types-and-guidelines)

**How do I import AutoCAD models?**

Currently DWG files are not supported. To import an AutoCAD file, export the
model as FBX from AutoCAD, and then define the textures in Blender or 3DS Max.
Export again as FBX and use the [!include[pn-import-tool](../includes/pn-import-tool.md)] cloud option.

Still need help? Try our [user forums](https://community.dynamics.com/365/layout).

### See also
[Overview of Layout](index.md)<br/>
[Device options and technical requirements](requirements.md)<br/>
[Try or buy, and deploy](../licensing/buy-and-deploy.md)<br/>
[User Guide](user-guide.md)<br/>
[How-to videos](https://go.microsoft.com/fwlink/p/?linkid=2021489)<br/>
