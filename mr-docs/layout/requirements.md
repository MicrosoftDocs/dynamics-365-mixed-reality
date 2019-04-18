---
author: ornellaalt
description: Device options and technical requirements for Dynamics 365 Layout
ms.author: ornella
ms.date: 4/18/2019
ms.service: crm-online
ms.topic: article
title: Device options and technical requirements for Dynamics 365 Layout
ms.reviewer: v-brycho
---

# Device options and technical requirements for Dynamics 365 Layout

[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-layout](../includes/pn-dyn-365-layout.md)] works with a [!include[pn-hololens](../includes/pn-hololens.md)], or with a [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Mixed Reality immersive headset with motion controllers.

## HoloLens requirements

| **OS requirements**          | **Details**                                                                                                                           |
|------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Build 10.0.17134.77 or later | See [Update HoloLens](https://support.microsoft.com/help/12643/hololens-update-hololens) for instructions on upgrading to this build. |

> [!NOTE]
> You can use the [!include[pn-hololens](../includes/pn-hololens.md)] clicker with [!include[pn-layout](../includes/pn-layout.md)] but it has limited functionality. You can use the clicker to do menu selections and to scan a room, but you can't use it to manipulate objects.


## Windows Mixed Reality headset requirements

| **Requirements**                          | **Details**                                                                                                                                                                                                                                                                                                                          |
|-------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC with build 17134.0 or later | The [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC hardware must be able to support the headset. See [Windows Mixed Reality PC hardware guidelines](https://support.microsoft.com/en-us/help/4039260/windows-10-mixed-reality-pc-hardware-guidelines) for specific hardware requirements. We recommend following the [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Mixed Reality Ultra hardware guidelines. |
| Motion controllers                        | Motion controllers are hardware accessories that allow users to take action in mixed reality. See [Motion controllers](https://docs.microsoft.com/en-us/windows/mixed-reality/motion-controllers) to learn more.                                                                                                                     |

Technical requirements
----------------------

| **Requirements**                   | **Details**                                                                                                                                                                                                                                                                                                                                                                                             | **Learn more**                                                                                                                                                |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!include[pn-azure-active-directory](../includes/pn-azure-active-directory.md)] ([!include[pn-azure](../includes/pn-azure.md)] AD)  | Required to sign in to [!include[pn-layout](../includes/pn-layout.md)] and for app distribution through the [Microsoft Store for Business](https://docs.microsoft.com/en-us/microsoft-store/sign-up-microsoft-store-for-business).                                                                                                                                                                                                               | [Get started with Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/get-started-azure-ad)                                                     |
| Network connectivity               | Internet access is required to download the app and to use all of its features. There are no bandwidth requirements.                                                                                                                                                                                                                                                                                    |                                                                                                                                                               |
| Apps for sharing    | Video calling or screen sharing requires a separate app, such as [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-remote-assist](../includes/pn-dyn-365-remote-assist.md)] on [!include[pn-hololens](../includes/pn-hololens.md)], or Skype or Skype for Business on immersive headsets. <br> <br>  A [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PC that meets the [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Mixed Reality Ultra specifications is also required for video calling or screen sharing when using [!include[pn-layout](../includes/pn-layout.md)] with an immersive headset.                                                                                                                                                                                                               | [Remote Assist](../remote-assist/user-guide.md) <br> <br>  [Windows Mixed Reality PC hardware guidelines](https://support.microsoft.com/en-us/help/4039260/windows-10-mixed-reality-pc-hardware-guidelines)                     |               
| [!include[pn-dyn-365-import-tool](../includes/pn-dyn-365-import-tool.md)] | The [!include[pn-import-tool](../includes/pn-import-tool.md)] runs on [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] 10 PCs, and is required to transfer existing 3D models from your PC to [!include[pn-layout](../includes/pn-layout.md)], so they can be viewed and edited from the [!include[pn-hololens](../includes/pn-hololens.md)] or immersive headsets. The [!include[pn-import-tool](../includes/pn-import-tool.md)] is also required to transfer [!include[pn-visio](../includes/pn-visio.md)] space dimensions to the [!include[pn-hololens](../includes/pn-hololens.md)] or immersive headsets. | [Import Tool](https://docs.microsoft.com/en-us/dynamics365/mixed-reality/import-tool)    |

### See also
[Try Layout for free](try-layout-free.md)<br/>
[Buy and deploy Layout](buy-and-deploy-layout.md)<br>
[User Guide](user-guide.md)<br/>
[How-to videos](https://go.microsoft.com/fwlink/p/?linkid=2021489)<br/>
[FAQ](faq.md)<br/>
