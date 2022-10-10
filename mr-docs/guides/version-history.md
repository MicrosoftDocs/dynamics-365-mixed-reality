---
author: Mamaylya
description: Describes older features for Dynamics 365 Guides, organized by release date
ms.author: mamaylya
ms.date: 04/05/2022
ms.topic: reference
title: Version history for Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Version history for Dynamics 365 Guides

This article provides a version history for Microsoft Dynamics 365 Guides features for all waves **except the current wave**. For current wave features, see [What's new in Dynamics 365 Guides](new.md). To see a comprehensive list of released and upcoming features for all waves, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>, which summarize early access features, preview features, monthly general availability enhancements, and bug fixes.

## 2022 Release Wave 1

## August 10, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|704.2207.27002|
|HoloLens app (HoloLens 2 only)|704.2207.27002|
|Solution|700.4.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2022wave1/guides/dynamics365-guides/grant-guide-access-third-parties" target="_blank">Grant guide access to third parties</a>| No |<a href="/dynamics365/mixed-reality/guides/admin-add-guest-user" target="_blank">Add a guest user</a>|
| Automatically update the HoloLens app to stay in sync with the latest solution version| Yes |<a href="/dynamics365/mixed-reality/guides/setup-step-three" target="_blank">Download the PC and HoloLens apps</a>|

> [!NOTE]
> You must be a system administrator to update the Dynamics 365 Guides solution. 

### Bugs fixed and other improvements

- Fixed issue with QR code detection

## June 29, 2022

Version 703.2206.27001 of the HoloLens app provides a bug fix for a permissions issue in the June 9 release related to Microsoft Intune. 

## June 9, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|703.2206.6001.0|
|HoloLens app (HoloLens 2 only)|703.2206.6001.0|
|Solution|700.3.0.1 |

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2022wave1/guides/dynamics365-guides/search-across-all-folders-database-instance-find-guide" target="_blank">Search across all folders in the database (instance) to find a guide</a>| No |<a href="/dynamics365/mixed-reality/guides/pc-app-find-guide" target="_blank">Find a guide in the PC app</a>|
| <a href="/dynamics365-release-plan/2022wave1/guides/dynamics365-guides/fix-guides-that-wont-load-due-accidental-deletion-tasks-or-steps-outside-app" target="_blank">Fix guides that won't load due to accidental deletion of tasks or steps outside the PC app</a>| No |<a href="/dynamics365/mixed-reality/guides/corrupted-guide" target="_blank">Fix a corrupted guide</a>|

> [!NOTE]
> You must be a system administrator to update the Dynamics 365 Guides solution. 

### Bugs fixed and other improvements

- Reduced number of “Out of Memory” crashes on HoloLens 2.
-	Adjusted the default microphone volume for calls recorded using Mixed Reality Capture. The default volume is now lower.
-	Fixed issue with ```<I>``` (capital I) tag not rendering italicized text correctly.  
-	Fixed issue with most recent version of a 3D model not being shown in a guide when a model was uploaded. The cached version of the 3D model is now cleared and updated when a new model is uploaded.
-	Fixed issue with Hebrew fallback font not rendering correctly in some scenarios.

## April 5, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|702.2203.31001|
|HoloLens app (HoloLens 2 only)|702.2203.31001|
|Solution|700.2.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/planned-features" target="_blank">New Guide Author Session table tracks interactions each time a user in Authoring mode opens, navigates, or closes a guide.</a>| Yes |<a href="/dynamics365/mixed-reality/guides/analytics-overview" target="_blank">Analytics overview</a>|

### Bugs fixed and other improvements

- Stability improved when saving guides with many steps and 3D content references.
- After a call has ended, the user will see the **Activities** menu in their view so that they can choose their next action.
- A banner notification is presented when connecting to a call while viewing a guide.

## 2021 Release Wave 2

## February 2, 2022

Version 701.2201.31001 of the PC and HoloLens apps provides bug fixes for both apps. To use the updated apps, you'll need Dynamics 365 Guides solution version 700.0.0.1 or later. 

## January 26, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|701.2201.20001|
|HoloLens app (HoloLens 2 only)|701.2201.20001|
|Solution|700.1.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/new-mr-app-sessions-table-tracks-success-dynamics-365-guides-organization" target="_blank">New MR App Sessions table tracks success of Dynamics 365 Guides in your organization</a>| Yes |<a href="/dynamics365/mixed-reality/guides/developer-entity-reference" target="_blank">Microsoft Dataverse table (entity) reference</a>|


### Bugs fixed and other improvements

- Improved reliability of Azure Object Anchors

## November 8, 2021

|Item|Version|
|-------------------------|--------------------------------|
|PC app|700.2111.3001|
|HoloLens app (HoloLens 2 only)|700.2111.3001|
|Solution|700.0.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/updated-user-experience-leveraging-hololens-2-instinctual-interactions" target="_blank">Touch menu for moving between activities and navigating lists of information</a>| Yes |<a href="/dynamics365/mixed-reality/guides/main-menu" target="_blank">Use the Main menu to start an activity</a>|
| <a href="/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/make-calls-directly-dynamics-365-guides-hololens-app" target="_blank">Make calls directly (Preview) from Dynamics 365 Guides</a>| Yes |<a href="/dynamics365/mixed-reality/guides/make-call" target="_blank">Make a call (Preview) in the Dynamics 365 Guides HoloLens app</a>|
| <a href="/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/ability-create-very-long-guides" target="_blank">Ability to create very long guides</a>| No |<a href="/dynamics365/mixed-reality/guides/hololens-app-place-holograms" target="_blank">Place and manipulate holograms in the Dynamics 365 Guides HoloLens app</a>|

> [!NOTE]
> If you have created any custom security roles, make sure to update those custom roles to match the permissions for relevant Dynamics 365 Guides Security roles (Author, Operator, Restricted Author, Restricted Operator) so that any custom roles have access to the new MR App Session table.

### Bugs fixed and other improvements

- Improved PC app stability around step deletion
- Fixed unsupported scenario that allowed users to specify a trigger style

## 2021 Release Wave 1

### August 30 2021

|Item|Version|
|-------------------------|--------------------------------|
|PC app|604.2108.20001|
|HoloLens app (HoloLens 2 only)|604.2108.20001|
|Solution|600.4.0.2|

#### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/select-multiple-animations-customize-animation-settings" target="_blank">Select from multiple animations and customize animation settings</a>| Yes |<a href="/dynamics365/mixed-reality/guides/hololens-app-orientation#change-animation-options" target="_blank">- Change animation options</a><br><a href="https://doc.babylonjs.com/extensions/Exporters/3DSMax_to_glTF#single-animation-clip" target="_blank">- Work with multiple animations in a single 3DS MAX model</a>|

####  Bugs fixed and other improvements

- Fixed search functionality in Offline mode
- Improved accessibility, generally
- Updated the instructions in the default anchoring mode

###  July 26, 2021

|Item|Version|
|-------------------------|--------------------------------|
|PC app|603.2107.20001.0|
|HoloLens app (HoloLens 2 only)|603.2107.20001.0|
|Solution|600.3.0.1|

#### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/leverage-azure-object-anchors-automatically-align-guide-content-real-world-objects" target="_blank">Leverage Azure Object Anchors to automatically anchor your guide content to real-world objects Preview</a>| Yes |- <a href="/dynamics365/mixed-reality/guides/pc-app-anchor-azure-object" target="_blank">Anchor a guide by using Azure Object Anchors</a><br>- <a href="https://cloudblogs.microsoft.com/dynamics365/bdm/2021/05/05/improve-on-the-job-guidance-with-dynamics-365-guides-and-azure-object-anchors/" target="_blank">Blog: Improve on-the-job guidance with Dynamics 365 Guides and Azure Object Anchors</a>|

#### Bugs fixed and other improvements

- Improved caching of guides for a better offline experience
- Fixed privilege validation issue for folders on HoloLens
- Improved the PC authoring app to better align with accessibility requirements

### June 29, 2021

|Item|Version|
|-------------------------|--------------------------------|
|PC app|602.2106.19001|
|HoloLens app (HoloLens 2 only)|602.2106.19001|
|Solution|600.2.0.2|

#### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/folders-pc-hololens-apps" target="_blank">Folders in PC and HoloLens apps</a>| No |<a href="/dynamics365/mixed-reality/guides/create-guide" target="_blank">Create a guide</a>|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/consolidated-content-view-guides-model-driven-app" target="_blank">Consolidated content view in the Guides model-driven app</a>| Yes |<a href="/dynamics365/mixed-reality/guides/admin-access-assign#share-a-guide-with-someone-else" target="_blank">Assign ownership of a guide</a>|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/reworked-notifications-accessibility" target="_blank">Reworked notifications for accessibility</a>| No |None|

#### Bugs fixed

- Space planning 3D collection is now fully localized
- Accessibility bug fixes
- Improvement to Restricted Author role to allow users to create guides from the Guides model-driven app and the PC app
- Improvements to deep linking

### May 4, 2021

#### Version info

|Item|Version|
|-------------------------|--------------------------------|
|PC app|601.2104.29001.0|
|HoloLens app (HoloLens 2 only)|601.2104.29001.0|
|Solution|600.1.0.1|

#### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/prepare-folders-guides-list-dynamics-365-guides-model-driven-app-admins" target="_blank">Prepare folders for the Guides list in the Dynamics 365 Guides model-driven app (for admins)</a>| Yes |<a href="/dynamics365/mixed-reality/guides/admin-create-folders" target="_blank">Organize guides into folders in Dynamics 365 Guides (for admins)</a>|
| <a href="/dynamics365-release-plan/2021wave1/finance-operations/dynamics365-guides/measure-lengths-angles-new-3d-toolkit-shapes" target="_blank">Measure lengths and angles with new 3D toolkit shapes</a>| Yes |<a href="/dynamics365/mixed-reality/guides/create-steps-assign-media" target="_blank">Add a 3D model from the 3D toolkit</a>|

#### Bugs fixed

- Fix for PC app crashing when selecting **Cancel** button after selecting anchor method
-	Fix for Guide Session records not created in Restricted Operator mode 
-	Fix for incorrect date shown in **Date Modified** field (**All** list)
-	Fix for Power BI visual not appearing after guide run through and step deletion

### April 1, 2021

> [!IMPORTANT]
> HoloLens (1st gen) has entered Long Term Servicing State and is no longer supported on the latest versions of Dynamics 365 Guides. Customers on HoloLens (1st gen) can continue using the last supported app version (600.2103.19001) released on April 1, 2021. This version of the app is compatible with all 500 solution versions up to and including 600.0.0.1, also released on April 1, 2021. To continue using HoloLens (1st gen), existing customers should not upgrade to a solution version later than 600.0.0.1. Solution version 600.0.0.1 is no longer available for download for new HoloLens 1 customers.

#### Version info

|Item|Version|
|-------------------------|--------------------------------|
|PC app|600.2103.19001|
|HoloLens app|600.2103.19001|
|Solution|600.0.0.1|

## 2020 Release Wave 2

### February 25, 2021

Version 504.2102.24001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 500.4.1.2 include the following new features.

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/deactivate-images-videos-3d-models-pc-app" target="_blank">Deactivate images, videos, and 3D models from the PC app</a> | Yes |<a href="/dynamics365/mixed-reality/guides/pc-app-deactivate-guide" target="_blank">Deactivate a guide or specific guide content</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/use-filters-find-guides-more-quickly-hololens-2" target="_blank">Use filters to find guides more quickly on HoloLens 2</a> | No |<a href="/dynamics365/mixed-reality/guides/find-guide" target="_blank">Find a guide to use in the HoloLens app</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/planned-features" target="_blank">Support for security permissions at team level</a> | Yes |*Content in progress*|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/planned-features" target="_blank">Performance improvements in loading list of guides</a> | No ||

### February 3, 2021

Version 503.2102.2001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 500.3.1.2 include the following new features.

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/extend-analytics-capabilities-guides-insights" target="_blank">Extend analytics capabilities with new guide operation data tables</a> | Yes |<a href="/dynamics365/mixed-reality/guides/analytics-overview" target="_blank">Overview of analyzing and integrating Dynamics 365 Guides operations data</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/gain-insights-into-guide-usage-updated-guides-analytics-power-bi-reports" target="_blank">Gain insights into guide usage with the updated Guides Analytics Power BI reports</a> | Yes |<a href="/dynamics365/mixed-reality/guides/analytics-ga-reports" target="_blank">Take a tour of Guides Analytics reports</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/improvement-how-data-stored-dataverse" target="_blank">Improvement in how data is stored in the Microsoft Dataverse</a> | Yes |<a href="https://community.dynamics.com/365/guides/f/dynamics-365-guides-forum/413710/information-about-guides-version-500-3-1-x-update-for-integrators" target="_blank">Information about Guides version 500.3.1.x update for integrators</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/narrated-instruction-text-through-hololens" target="_blank">Narrated instruction text through HoloLens</a> | No |<a href="/dynamics365/mixed-reality/guides/operator-narrator" target="_blank">Have HoloLens narrate instructions</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/updated-dynamics-365-guides-demo" target="_blank">Updated Dynamics 365 Guides demo</a> | No ||

> [!IMPORTANT]
> If you're an integrator and you have used custom security roles in your implementations, you'll need to edit those security roles. See <a href="https://community.dynamics.com/365/guides/f/dynamics-365-guides-forum/413710/information-about-guides-version-500-3-1-x-update-for-integrators" target="_blank">information about version 500.3.1.x for integrators</a>.

### December 8, 2020

Version 502.2011.28001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 500.2.1.2 include the following new feature.

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/improved-experience-finding-guides-pc-app" target="_blank">Improved experience finding guides in the PC app</a> | No |<a href="/dynamics365/mixed-reality/guides/create-guide" target="_blank">Create or find a guide in the PC app</a>|

> [!IMPORTANT]
> **Important information about HoloLens 1:** In Dynamics 365 Guides version 502.2011.28001 (December 8, 2020 release) and later, HoloLens operating system version 10.0.17134 (Redstone 4) is no longer supported. This version of the operating system is used only on HoloLens 1. HoloLens 1 customers must upgrade to HoloLens version 10.0.17763 or later to continue to receive the latest updates. Work with your IT admin to update your HoloLens operating system. If you choose not to upgrade, you can continue to use the current version of Dynamics 365 Guides that is already installed on the device. However, HoloLens version 10.0.17763 or later is required to install Dynamics 365 Guides on any new or refactored HoloLens 1 device.

### October 27, 2020

Version 501.2010.17001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 500.1.1.0 include the following new feature.

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/support-government-community-cloud" target="_blank">Dynamics 365 Guides Government Community Cloud</a> | No |<a href="/dynamics365/mixed-reality/guides/gcc" target="_blank">Dynamics 365 Guides US Government</a>|

### October 1, 2020

Version 500.2009.23001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 500.0.1.1  include the following new features.

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/create-guides-that-support-branching-flows" target="_blank">Create guides that support non-linear (branching) workflows </a> | Yes |<a href="/dynamics365/mixed-reality/guides/pc-app-branching" target="_blank">Add a branch in a guide to create a non-linear workflow</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/use-trigger-branch-specific-step" target="_blank">Use a trigger to branch to a specific step </a> | Yes |<a href="/dynamics365/mixed-reality/guides/pc-app-trigger" target="_blank">Create a trigger for step navigation in the PC app</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/activate-trigger-when-operators-hand-enters-trigger-area" target="_blank">Activate a trigger when the operator's hand enters the trigger area </a> | No |<a href="/dynamics365/mixed-reality/guides/pc-app-trigger" target="_blank">Create a trigger for step navigation in the PC app</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/copy-paste-position-orientation-scale-3d-model" target="_blank">Copy and paste the position, orientation, and scale of a 3D model </a> | No |<a href="/dynamics365/mixed-reality/guides/hololens-app-orientation#copy-and-paste-a-3d-models-position" target="_blank">Copy and paste a 3D model's position</a>|
| <a href="/dynamics365-release-plan/2020wave2/finance-operations/dynamics365-guides/copy-dynamics-365-guides-content-one-common-data-service-instance-another" target="_blank">Copy Dynamics 365 Guides content from one Microsoft Dataverse instance to another </a> | No |<a href="/dynamics365/mixed-reality/guides/migrate" target="_blank">Migrate Dynamics 365 Guides content from one Microsoft Dataverse instance to another</a>|

## 2020 Release Wave 1

### September 2, 2020

Version 404.2009.2003 of the PC app and version 404.2009.2004 of the HoloLens app fixed a bug introduced in the August 25 release that prevented some guides from opening and displayed a misleading error message. You don't need to update the Dynamics 365 Guides solution to get this update.

### August 25, 2020

Version 404.2008.19001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 400.0.4.31 include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|------|
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/use-spatial-triggers-go-forward-or-backward-guide" target="_blank">Use spatial triggers to go forward or backward in a guide</a> | Yes |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/new-security-roles-restrict-access-guides" target="_blank">New security roles to restrict access to guides</a> | Yes |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/preview-image-video-or-3d-model-new-properties-tab" target="_blank">Preview an image, video, or 3D model in the new Properties tab</a> | No |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/back-button-behavior-changed-return-operator-previously-visited-step" target="_blank">Back button behavior changed to return operator to the previously visited step</a> | No |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/step-card-ui-update" target="_blank">Step card UI update</a> | No |

### August 4, 2020

Version 403.2008.3001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 400.0.3.36 include the following new feature.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|------|
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/use-voice-operate-guides-hololens" target="_blank">Use voice to operate your guides on HoloLens</a> | No |

#### Other updates

This release also includes the following fixes and updates:

- Added <a href="/dynamics365/mixed-reality/guides/migrate" target="_blank">Content Migration Tool</a> to move content from one Microsoft Dataverse instance to another.

- Addressed an issue that affected some PCs when the PC app was used to upload files.

- Improvements to deeplink functionality and embedded links in QR codes for quick launch of a guide.

### July 7, 2020

Version 402.2007.7001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 400.0.2.66 include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|------|
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/operators-use-previously-opened-guides-hololens-when-offline" target="_blank">Operators can use any previously opened guides on HoloLens when offline</a> | No |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/planned-features" target="_blank">Filter Power BI dashboard data by Author or Operator role</a> | No |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/improved-hologram-alignment-real-world-during-mixed-reality-capture-hololens-2" target="_blank">Improved hologram alignment with real world during Mixed Reality Capture on HoloLens 2</a> | No |

#### Other update

This release also includes the following fix:

- **Embedded link in QR code.** There was an issue with the deeplink functionality where the embedded link in a QR code didn't link to the correct guide or step.

### May 26, 2020

Version 401.2005.21001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and solution version 400.0.0.18 include the following new feature. Version 401.2005.21001 of the HoloLens and PC apps are only compatible with version 400.0.0.18 (April 28th) or later. <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">See the apps and solution compatibility table for more details</a>. 

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|------|
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/improved-user-experience-audio-feedback" target="_blank">Improved user experience with audio feedback</a> | No |

### May 14, 2020

Version 400.2005.13001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps fixed a bug introduced in the April 28 release that prevented some model animations from playing on [!include[pn-hololens](../includes/pn-hololens.md)]. You don't need to update the Dynamics 365 Guides solution to get this update.

### April 28, 2020

Version 400.2004.24002.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 400.0.0.18 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|------|
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/access-dynamics-365-guides-content-through-common-data-service-entities" target="_blank">Access Dynamics 365 Guides content through Microsoft Dataverse entities</a> | Yes |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/integrate-asset-management-module-dynamics-365-supply-chain-management" target="_blank">Integrate the Asset Management module of Dynamics 365 Supply Chain Management with Dynamics 365 Guides</a> | No |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/rename-guides-pc-app" target="_blank">Rename guides in the PC app</a> | No |

#### Other updates: Example guide is deprecated

From the April 28, 2020 release onward, the Example guide is deprecated and no longer deployed to new instances. If users have already installed the Example guide in a non-English deployment, they won't be able to open the guide. When attempting to open a localized Example guide, users will be redirected back to the **Guides** list.

### April 1, 2020

Version 305.2003.28001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 300.0.5.127 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|------|
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/restrict-access-guides-that-aren’t-ready-use-through-publishing-process" target="_blank">Restrict access to guides that aren't ready to share with operators</a> | No |
| <a href="/dynamics365-release-plan/2020wave1/mixed-reality/dynamics365-guides/planned-features" target="_blank">Sort items in the PC app gallery by recently added, or by name</a> | No |

## 2019 Release Wave 2

### February 25, 2020

Version 304.2002.25001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 300.0.4.139 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/anchor-guide-qr-code" target="_blank">Anchor guides by using QR codes</a> | Yes |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/create-copy-link-guide-or-step" target="_blank">Create and copy a link to a guide or step</a> | No |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/open-app-created-power-apps-step" target="_blank">Open an app created in Power Apps from a step</a> | Yes |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/deactivate-reactivate-or-delete-guide" target="_blank">Deactivate, reactivate, or delete a guide</a> | No |

### January 28, 2020

Version 303.2001.21001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 300.0.3.137 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/instinctual-interactions-authors-hololens-2" target="_blank">Instinctual interactions for authors on HoloLens 2</a> | No |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/open-website-hololens-app" target="_blank">Open a website from the HoloLens app</a> | Yes |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/assign-operator-author-roles-users" target="_blank">Assign Author and Operator roles to users</a> | Yes |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/drag-drop-multiple-files-into-pc-app-gallery" target="_blank">Drag and drop multiple files to the PC app gallery</a> | No |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/additional-resources-help-menu-pc-app" target="_blank">Additional resources in Help menu for PC app</a> | No |

#### Other updates

- The media panel is automatically resized to fit the attached media, which is optimized for the [!include[pn-hololens](../includes/pn-hololens.md)] field of view.

- The **Recent guides** list now shows only your recently opened guides.

- Hologram stabilization has been improved and optimized for HoloLens 2.

- Documentation has been reorganized so that it's easier to find information for specific roles (admin, author, and operator).

### October 29, 2019

Version 301.1910.24001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 300.0.1.115 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/support-node-based-animations" target="_blank">Support for node-based animations</a> | No |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/turn-animations-or-off" target="_blank">Turn animations on or off</a> | No |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/support-stl-ply-file-formats-3d-models" target="_blank">Support for STL and PLY file formats for 3D models</a> | No |

#### Other updates

- Removed different sizes for the same model from the 3D toolkit (this change requires a solution update). Because authors can now resize models, the different sizes are no longer required.

- Updated the Follow (tag-along) behavior of the Step card to be consistent with the Windows Holographic OS (Shell) behavior where the Step card follows you when the option is turned on.

### October 1, 2019

Version 200.1909.24001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 200.0.0.107 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/try-demo-dynamics-365-guides" target="_blank">Try a demo of Dynamics 365 Guides</a> | Yes |
| Customer satisfaction surveys | No |
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/opt-out-collecting-dynamics-365-guides-data" target="_blank">Opt out of collecting Dynamics 365 Guides data</a> | Yes |

#### Other updates

The October 1 release also includes refactoring of code for hologram positions to enhance overall performance and enable future improvements. You may notice that the position of some imported models, which have had scale applied to them, might be shifted. You will need to re-position those 3D models. This does not impact the position of models from the 3D toolkit.

## 2019 Release Wave 1

### August 27, 2019

Version 104.1908.24001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 104.1908.0.117 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/accessibility" target="_blank">Accessibility enhancements for PC app</a> | No |
| Improved hologram manipulation | No |
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/localization" target="_blank">Support for additional languages</a> | Yes |

### August 6, 2019

[!include[pn-hololens](../includes/pn-hololens.md)] app version 104.1908.2001.0 fixes an issue in the July 23 release of the [!include[pn-hololens](../includes/pn-hololens.md)] app that prevented the list of guides from being shown in the [!include[pn-hololens](../includes/pn-hololens.md)] application for Europe, Middle East, and Asia-based customers. We also released an updated version of the Power BI reporting template that fixes a bug related to missing data causing the report to break.

To get this update, you just have to update the [!include[pn-hololens](../includes/pn-hololens.md)] app from [!include[cc-microsoft](../includes/cc-microsoft.md)] Store. You don't have to update the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution. For the Power BI report, visit <a href="https://aka.ms/guidesreport" target="_blank">https://aka.ms/guidesreport</a>.

### July 23, 2019

Version 104.1907.19001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps and version 104.1907.0.33 of the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] solution include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/dynamics365-release-plan/2019wave2/mixed-reality/dynamics365-guides/integration-dynamics-365-field-service" target="_blank">Integration with Dynamics 365 Field Service</a> | Yes |

Customers interested in previewing integration with [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] need to have an existing [!include[pn-dyn-365](../includes/pn-dyn-365.md)] instance with [!include[pn-dyn-365-field-service](../includes/pn-dyn-365-field-service.md)] version 8.6.0.183 or later installed. 

Visit aka.ms/getguides for steps to upgrade.

### July 9, 2019

Version 103.1907.4001.0 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps includes the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/pc-ux" target="_blank">PC app is fully responsive across various screen sizes</a> | No |
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/pc-ux" target="_blank">Left navigation menu makes navigation faster</a> | No |
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/hololens-ux" target="_blank">Gaze-dwell interactions consistently placed for easier selection</a> | No |
|3D models loaded for each step to improve performance on HoloLens| No |
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/new" target="_blank">What's New panel</a> | No |
 
### June 3, 2019

Version 103.1905.31001 of the PC and [!include[pn-hololens](../includes/pn-hololens.md)] apps include the following new features.

| Feature | Solution update required? |
|----------------------------------------------------------------------------------------|-------|
| <a href="/business-applications-release-notes/April19/dynamics365-mixed-reality/microsoft-dynamics365-guides/anchoring-improvements" target="_blank">Switch anchoring method at any time</a> | Yes |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
