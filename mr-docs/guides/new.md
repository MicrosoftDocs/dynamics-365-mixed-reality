---
author: Mamaylya
description: Describes the new features in Dynamics 365 Guides, organized by release date.
ms.author: mamaylya
ms.date: 07/27/2021
ms.topic: reference
title: What's new in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Guides

> [!IMPORTANT]
> The Dynamics 365 Guides HoloLens and PC apps released on May 4th or later require an April 1 or later version of the Microsoft Dataverse solution (version 600 or later). 
>
> If you choose not to update the solution and your PC and HoloLens apps, there's no impact.  
>
> Please work with your IT admin to schedule the installation update. <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">See instructions for updating the solution</a>. 

This page provides details about the latest releases of [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] organized by release date. To see a comprehensive list of released and upcoming features, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>.

> [!NOTE]
> If you have feature requests or suggested improvements, you can send them to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] team at <a href="https://aka.ms/GuidesIdeas" target="_blank" data-linktype="absolute-path">https://aka.ms/GuidesIdeas</a>.

## July 27, 2021

|Item|Version|
|-------------------------|--------------------------------|
|PC app|603.2107.20001.0|
|HoloLens app (HoloLens 2 only)|603.2107.20001.0|
|Solution|600.3.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/leverage-azure-object-anchors-automatically-align-guide-content-real-world-objects" target="_blank">Leverage Azure Object Anchors to automatically anchor your guide content to real-world objects (Preview)</a>| No |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/pc-app-anchor-azure-object" target="_blank">Anchor a guide by using Azure Object Anchors</a>|

### Bugs fixed and other improvements

- Improved caching of guides for a better offline experience
- Fixed privilege validation issue for folders on HoloLens
- Improved the PC authoring app to better align with accessibility requirements

## June 29, 2021

|Item|Version|
|-------------------------|--------------------------------|
|PC app|602.2106.19001|
|HoloLens app (HoloLens 2 only)|602.2106.19001|
|Solution|600.2.0.2|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/folders-pc-hololens-apps" target="_blank">Folders in PC and HoloLens apps</a>| No |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/create-guide" target="_blank">Create a guide</a>|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/consolidated-content-view-guides-model-driven-app" target="_blank">Consolidated content view in the Guides model-driven app</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/admin-access-assign#share-a-guide-with-someone-else" target="_blank">Assign ownership of a guide</a>|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/reworked-notifications-accessibility" target="_blank">Reworked notifications for accessibility</a>| No |None|

### Bugs fixed

- Space planning 3D collection is now fully localized
- Accessibility bug fixes
- Improvement to Restricted Author role to allow users to create guides from the Guides model-driven app and the PC app
- Improvements to deep linking

## May 4, 2021

### Version info

|Item|Version|
|-------------------------|--------------------------------|
|PC app|601.2104.29001.0|
|HoloLens app (HoloLens 2 only)|601.2104.29001.0|
|Solution|600.1.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/prepare-folders-guides-list-dynamics-365-guides-model-driven-app-admins" target="_blank">Prepare folders for the Guides list in the Dynamics 365 Guides model-driven app (for admins)</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/admin-create-folders" target="_blank">Organize guides into folders in Dynamics 365 Guides (for admins)</a>|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/measure-lengths-angles-new-3d-toolkit-shapes" target="_blank">Measure lengths and angles with new 3D toolkit shapes</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/create-steps-assign-media" target="_blank">Add a 3D model from the 3D toolkit</a>|

### Bugs fixed

- Fix for PC app crashing when selecting **Cancel** button after selecting anchor method
-	Fix for Guide Session records not created in Restricted Operator mode 
-	Fix for incorrect date shown in **Date Modified** field (**All** list)
-	Fix for Power BI visual not appearing after guide run through and step deletion

## April 1, 2021

> [!IMPORTANT]
> HoloLens (1st gen) has entered Long Term Servicing State and is no longer supported on the latest versions of Dynamics 365 Guides. Customers on HoloLens (1st gen) can continue using the last supported app version (600.2103.19001) released on April 1, 2021. This version of the app is compatible with all 500 solution versions up to and including 600.0.0.1, also released on April 1, 2021. To continue using HoloLens (1st gen), existing customers should not upgrade to a solution version later than 600.0.0.1. Solution version 600.0.0.1 is no longer available for download for new HoloLens 1 customers.

### Version info

|Item|Version|
|-------------------------|--------------------------------|
|PC app|600.2103.19001|
|HoloLens app|600.2103.19001|
|Solution|600.0.0.1|

> [!TIP]
> Looking for earlier features? Go to [version history for Dynamics 365 Guides](./version-history.md). 


## See also

- <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>

- <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a>

- <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">Check compatibility between Dynamics 365 Guides solution and PC/HoloLens apps</a>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
