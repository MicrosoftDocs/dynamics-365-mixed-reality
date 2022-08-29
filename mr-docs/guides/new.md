---
author: Mamaylya
description: Describes the new features in Dynamics 365 Guides, organized by release date.
ms.author: mamaylya
ms.date: 08/10/2022
ms.topic: reference
title: What's new in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

<br />

# What's new in Dynamics 365 Guides

This page provides details about the **current wave of features (April 2022 through September 2022)** for [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], organized by release date. To see a comprehensive list of released and upcoming features, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>. You can also <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">see a complete list of features organized by previous waves</a>. 

> [!IMPORTANT]
> Guides Dataverse solution version 700.2.0.1, which is now available, is a foundational change for key features in upcoming Dynamics 365 Guides releases and includes the new Guide Author Session table. Updated versions of the PC and HoloLens apps are available for the new solution and **require the 700.0.0.1 or newer solution.** Also, if you have created any custom security roles, **make sure to update those custom roles to match the permissions for relevant Dynamics 365 Guides Security roles (Author, Restricted Author) so that any custom roles have access to the Guide Author Session table.** Users with custom roles derived from the Author or Restricted Author security roles will be unable to log into the HoloLens and PC apps until the custom security roles are updated.  
> 
> If you choose not to update the solution and remain on the version 600 solution and compatible versions of the PC and HoloLens apps, there's no impact.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md). See the **Features** table below to determine if a new feature requires a solution update. 

If you have feature requests or suggested improvements, send them to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] team at <a href="https://aka.ms/GuidesIdeas" target="_blank" data-linktype="absolute-path">https://aka.ms/GuidesIdeas</a>.

## August 10, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|704.2207.27002|
|HoloLens app (HoloLens 2 only)|704.2207.27002|
|Solution|700.4.0.1|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2022wave1/guides/dynamics365-guides/grant-guide-access-third-parties" target="_blank">Grant guide access to third parties</a>| No |<a href="/dynamics365/mixed-reality/guides/admin-add-guest-user" target="_blank">Add a guest user</a>|
| Automatically update the HoloLens app to stay in sync with the latest solution version| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/setup-step-three" target="_blank">Download the PC and HoloLens apps</a>|

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
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2022wave1/guides/dynamics365-guides/search-across-all-folders-database-instance-find-guide" target="_blank">Search across all folders in the database (instance) to find a guide</a>| No |<a href="/dynamics365/mixed-reality/guides/pc-app-find-guide" target="_blank">Find a guide in the PC app</a>|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2022wave1/guides/dynamics365-guides/fix-guides-that-wont-load-due-accidental-deletion-tasks-or-steps-outside-app" target="_blank">Fix guides that won't load due to accidental deletion of tasks or steps outside the PC app</a>| No |<a href="/dynamics365/mixed-reality/guides/corrupted-guide" target="_blank">Fix a corrupted guide</a>|

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

> [!TIP]
> Looking for a list of earlier features? Go to <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>.

## See also

- <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>

- <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a>

- <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">Check compatibility between the Dynamics 365 Guides Dataverse solution and PC/HoloLens apps</a>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
