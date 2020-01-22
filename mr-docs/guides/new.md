---
author: makamat
description: Describes the new features in Dynamics 365 Guides, organized by release date
ms.author: makamat
ms.date: 01/28/2020
ms.service: crm-online
ms.topic: article
title: What's new in Dynamics 365 Guides
ms.reviewer: v-brycho
---

## What's new in Dynamics 365 Guides

This page provides details about the latest releases of [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] organized by release date. 

### January 28, 2020

The January 28 update includes the following new features:

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] now supports [!include[pn-hololens](../includes/pn-hololens.md)] 2 hand tracking to provide instinctual interactions for authors. Select and position holograms with direct touch, just like real objects. Use hand rays to interact with holograms when they're out of reach. On [!include[pn-hololens](../includes/pn-hololens.md)] 1, the app works the same as before since [!include[pn-hololens](../includes/pn-hololens.md)] 1 doesn’t support hand tracking. 

- Authors can add a website link to a step in a guide. Use a website link to display a PDF hosted on your server, show a form, or show data from your online IoT devices for the operator to review.

- Administrators can assign **Author** and **Operator** roles to users so that editing is only enabled for authors. 

- Drag and drop multiple files from your local file folder into the PC app gallery to import the files.

- Select the **Help** (question mark) button in the PC app to: 

  - Get quick access to video tutorials that show how to author, operate, or analyze guides.
  
  - Get phone numbers for customer support.
  
  - Provide feedback and ideas for the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] team. 
  
#### Other updates

- The media panel automatically resizes to fit the attached media, which optimizes for the [!include[pn-hololens](../includes/pn-hololens.md)] field of view. 

- The **Recent guides** list now shows only your recently opened guides.

- Hologram stabilization is improved and optimized for HoloLens 2. 

- Reorganized documentation to make it easier to find information for specific roles (admin, author, operator).

### October, 29, 2019

The [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] on October 29 brings highly requested features for content creators: 

- You can import models with node-based animations and use them in work instructions.

- Authors can turn animations on or off for 3D models.

- [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] now supports STL and PLY formats for 3D models.

To get this update, please upgrade to app version 301.1910.24001 and solution version 300.0.1.115.

We also:

- Removed different sizes for the same model in the 3D toolkit. Since authors can now resize models, the different sizes are not needed anymore.

- Updated the Follow (tag-along) behavior of the Step card to be consistent with the Windows Holograpic OS (Shell) behavior where the Step card follows you when the option is turned on.

### October 1, 2019

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] is now generally available (GA)! The October 1, 2019 updates for the PC app, HoloLens app, and Common Data Service solution need to be installed to continue using [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. Upgrades will continue to work with your preview license until it expires. To check your preview license expiration date, go to https:<i></i>//admin.microsoft.com/, and then select **Billing** in settings to ensure continuity.

New customers must acquire a new GA license. Please go to aka.ms/GetGuides for information on licenses, installation, and upgrades.

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app version 200.1909.24001 and solution version 200.0.0.107 include the following updates:

- **Try the demo.** You can now try an out-of-box sample guide on the HoloLens app without signing up for a license or authoring a guide yourself.

- **Customer satisfaction surveys.** We will occasionally ask you to rate your satisfaction with the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] to help us improve the product.

- **Opt out of sending data to Microsoft.** On both PC and HoloLens apps, for privacy reasons, you can turn off the ability to send telemetry data to Microsoft. 

- **Opt out of sending usage data to your organization.** To prevent usage data from showing in Power BI dashboards, administrators can now turn this off for specific users.

The October 1 release also includes refactoring of code for hologram positions to enhance overall performance and enable future improvements. You may notice that the position of some imported models, which have had scale applied to them, might be shifted. You will need to re-position those 3D models. This does not impact the position of models from the 3D toolkit.

### August 27, 2019
[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app version 104.1908.24001 and solution version 104.1908.0.117 includes the following updates:

- **Accessibility enhancements.** The PC application offers better color contrast and support for high-contrast mode for visually impaired users. Use the keyboard to tab through the user interface while using Narrator to read various authoring options. In preview mode, you can manipulate 3D models using the keyboard.

- **Improved hologram manipulation.** Holograms move more naturally as you place them in space, making it easier to accurately align holograms to the real world.

- **Support for additional languages**. The PC app and the HoloLens app now support the following languages: English (US, UK), French (France, Canada), German, Dutch (Netherlands), Spanish, Italian, Chinese (People’s Republic of China, Taiwan, Hong Kong SAR), Japanese, and Korean.

> [!NOTE]
> To get this update, you need to update the PC app and the [!include[pn-hololens](../includes/pn-hololens.md)] app from the [!include[cc-microsoft](../includes/cc-microsoft.md)] Store. Updating the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution is not mandatory, but you need to update it if you intend to use the app in the newly supported languages. 

### August 6, 2019
[!include[pn-hololens](../includes/pn-hololens.md)] app version 104.1908.2001.0 fixes an issue in the July 23rd release of the [!include[pn-hololens](../includes/pn-hololens.md)] app that prevented the list of guides from being shown in the [!include[pn-hololens](../includes/pn-hololens.md)] application for Europe, Middle East, and Asia-based customers. We also released an updated version of the Power BI reporting template that fixes a bug related to missing data causing the report to break.

To get this update, you only need to update the [!include[pn-hololens](../includes/pn-hololens.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app from the [!include[cc-microsoft](../includes/cc-microsoft.md)] Store. You don't need to update the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution. For the Power BI report, please visit https:<i></i>//aka.ms/guidesreport.

### July 23, 2019

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app version 104.1907.19001 and CDS solution version 104.1907.0.33 introduces integration with [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)]. **[!include[pn-field-service](../includes/pn-field-service.md)]** customers can now attach guides to service tasks in [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)]. When work orders are assigned to technicians, the technicians can launch the assigned guide in a dedicated **[!include[pn-field-service](../includes/pn-field-service.md)]** tab in the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] application and do their work.

Customers interested in previewing integration with [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] need to have an existing [!include[pn-dyn-365](../includes/pn-dyn-365.md)] Customer Engagement (CRM) instance with [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] version 8.6.0.183 or later. 

Visit aka.ms/getguides for steps to upgrade.

### July 9, 2019

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app version 103.1907.4001.0 brings a new look and feel to the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps. We improved the user experience and aligned it with the [!include[pn-dyn-365](../includes/pn-dyn-365.md)] family of apps. 
 
#### Improvements in this release

- The PC app is now fully responsive across various screen sizes. 

- The navigation menu on the left and bottom right of the PC app makes it much faster to navigate between guide content and guide anchor settings. 
 
- “Gaze-dwell” interactions on [!include[pn-hololens](../includes/pn-hololens.md)] are consistently placed on the left side of list items to make it easier to select while browsing. 

- 3D models are loaded for each step to improve performance on [!include[pn-hololens](../includes/pn-hololens.md)].
 
This **What's New** panel will continue to inform you of new and noteworthy features in each monthly release.

### June 3, 2019

[!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] app version 103.1905.31001 introduces an improved anchoring (alignment) experience for [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)]. The PC app doesn’t require you to choose an anchoring method before creating a guide so you can start creating content right away. You can also switch between anchoring methods after creating a guide. The PC app also provides better step-by-step guidance for choosing the appropriate method for anchoring mixed reality instructions to your workspace.

If you choose to create a guide using a digital anchor, you can now use a pre-set 3D model, so you don’t have to choose a 3D model 
before proceeding.

> [!NOTE]
> To take advantage of the new anchoring improvements, you must update the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution in the [!include[pn-dyn-365](../includes/pn-dyn-365.md)] 
admin center. For more information, see <a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a> or contact your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] administrator.

For more information on authoring a guide with the PC application, see <a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/pc-authoring" target="_blank">Use the PC authoring application to create a guide</a>.

