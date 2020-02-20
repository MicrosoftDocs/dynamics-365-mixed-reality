---
author: BryceHo
description: Known Issues with the Dynamics 365 Guides PC app
ms.author: makamat
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Known Issues with the Dynamics 365 Guides PC app
ms.reviewer: v-brycho
---

# Known issues with the Dynamics 365 Guides PC app

## I can't sign in

To sign in, you must use the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365](../includes/pn-dyn-365.md)] sign-in credentials for your organization. It will resemble: johndoe@contoso.onmicrosoft.com. You can't use a [!include[cc-microsoft](../includes/cc-microsoft.md)] account (used for Outlook.com, [!include[pn-ms-windows-short](../includes/pn-ms-windows-short.md)] Store, and so on) or your corporate credentials to sign in. 

If you see any of the following errors, contact your IT admin, or see the self-service documentation at <https://aka.ms/guidesdocs>:

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] isn't set up correctly, or you might not have permission to access it. Contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- Your client app version doesn't support your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution version. Update your client app, contact your admin, or see the [self-service documentation](https://aka.ms/guidesdocs).

- You don't have a license to use [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Contact your admin, or [sign up for a free trial subscription]().

## Staying on the account picker for more than 25 seconds during HoloLens sign-in will make it unresponsive

When you get to the screen where you can select between different saved accounts on [!include[pn-hololens](../includes/pn-hololens.md)], choose an option within 25 seconds. After 25 seconds, it becomes unresponsive, and you will need to restart the app. This issue has been fixed on RS5 but still exists on RS4 if you have that installed.

## "Create account" link when signing in with a new account doesn't work
When signing in with a brand new account on the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps, there is a link to create a new account:

![Sign-in screen](media/sign-in-screen.PNG "Sign-in screen")  
 
Please do not use this link to create an account–it doesn't work.

## I can't see guides that I created or guides created by my teammates

If you don't see any guides, either your internet connection is unstable, or you might have signed in to an instance that doesn't have any guides. First, check your internet connection. If you're connected, try signing in again, but this time make sure you sign into the instance that has the guides you were looking for. If you still don't see any guides, contact your administrator.

## I don't see media or 3D content that I uploaded to the app

When you upload content, at this time, the app doesn't automatically scroll to the place in the library where the content is uploaded. To find the content, go to the library (right side of the screen), and then select the appropriate tab (**3D parts**, **Pictures**, **Videos**, or **3D toolkit**).

The PC app shows notifications (in the top title bar) if there are any errors during uploading. Check to make sure your content is in the right file format. [Learn about supported file formats for Dynamics 365 Guides](create-steps-assign-media.md#what-file-formats-are-supported-for-3d-models-images-and-videos). 

If you still can't find your content, contact your administrator.

## I have an issue that isn't listed in these troubleshooting steps

Please contact customer service: [https://docs.microsoft.com/dynamics365/get-started/support/](https://docs.microsoft.com/dynamics365/get-started/support/). This page can also be found by signing in to your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] account and selecting the **Support** link.

## See also

[Known issues with Dynamics 365 Guides generally](known-issues.md)<br>
[Known issues with the HoloLens app](known-issues-hololens-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)

