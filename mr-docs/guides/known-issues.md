---
author: BryceHo
description: Known Issues with Dynamics 365 Guides
ms.author: makamat
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Known Issues with Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Known issues with Microsoft Dynamics 365 Guides

## Improvements for 3D model positioning in the October 1 release might shift models in guides that were created before October 1, 2019

The October 1 release includes refactoring of code for hologram positions to enhance overall performance and enable future improvements. You may notice that the position of some imported models, which have had scale applied to them, might be shifted. You will need to re-position those 3D models. This does not impact the position of models from the 3D toolkit.

## "Create account" link when signing in with a new account doesn't work
When signing in with a brand new account on the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps, there is a link to create a new account:

![Sign-in screen](media/sign-in-screen.PNG "Sign-in screen")  
 
Please do not use this link to create an account–it doesn't work.

## I can't see guides that I created or guides created by my teammates

If you don't see any guides, either your internet connection is unstable, or you might have signed in to an instance that doesn't have any guides. First, check your internet connection. If you're connected, try signing in again, but this time make sure you sign into the instance that has the guides you were looking for. If you still don't see any guides, contact your administrator.

## Text wrapping on PC and HoloLens might differ in rare cases

In rare cases, you might notice that text is wrapped on the step card view in [!include[pn-hololens](../includes/pn-hololens.md)] but not on the PC. This is because [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] renders fonts at different sizes for readability between PC and [!include[pn-hololens](../includes/pn-hololens.md)], and different widths of characters might cause them to go to the next line. To ensure this does not affect operator experience, validate the text on all steps on the [!include[pn-hololens](../includes/pn-hololens.md)] app before sharing your guides with operators.

## See also

[Known issues with the PC app](known-issues-pc-app.md)<br>
[Known issues with the HoloLens app](known-issues-hololens-app.md)<br>
[Dynamics 365 Guides FAQ](faq.md)

