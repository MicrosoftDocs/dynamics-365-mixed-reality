---
author: Mamaylya
description: Describes the new features in Dynamics 365 Guides, organized by release date.
ms.author: mamaylya
ms.date: 02/02/2022
ms.topic: reference
title: What's new in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Guides

This page provides details about the **current wave of features (October 2021 through March 2022)** for [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], organized by release date. To see a comprehensive list of released and upcoming features, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>. You can also <a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/version-history" target="_blank">see a complete list of features organized by previous waves</a>. 

> [!IMPORTANT]
> Guides Dataverse solution version 700.1.0.1, which is now available, is a foundational change for key features in upcoming Dynamics 365 Guides releases and includes the new MR App Session table. Updated versions of the PC and HoloLens apps are available for the new solution and **require the 700.0.0.1 or newer solution.** To install solution version 700.1.0.1, it's a good idea to first install solution version 700.0.0.1 if you haven’t already. Also, if you have created any custom security roles, **make sure to update those custom roles to match the permissions for relevant Dynamics 365 Guides Security roles (Author, Operator, Restricted Author, Restricted Operator) so that any custom roles have access to the new MR App Session table.**
> 
> If you choose not to update the solution and remain on the version 600 solution and compatible versions of the PC and HoloLens apps, there's no impact.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md). See the **Features** table below to determine if a new feature requires a solution update. 

If you have feature requests or suggested improvements, send them to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] team at <a href="https://aka.ms/GuidesIdeas" target="_blank" data-linktype="absolute-path">https://aka.ms/GuidesIdeas</a>.

## March 29, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|XXX|
|HoloLens app (HoloLens 2 only)|XXX|
|Solution|XXX|

### Features

| Feature | Solution update required? |How to|
|----------------------------------------------------------------------------------------|------|------------------------------------|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/planned-features" target="_blank">New XXX table XXX</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/developer-entity-reference" target="_blank">Microsoft Dataverse table (entity) reference</a>|

### Bugs fixed and other improvements

- XXX

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
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/planned-features" target="_blank">New MR App Sessions table tracks success of Dynamics 365 Guides in your organization</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/developer-entity-reference" target="_blank">Microsoft Dataverse table (entity) reference</a>|

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
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/updated-user-experience-leveraging-hololens-2-instinctual-interactions" target="_blank">Touch menu for moving between activities and navigating lists of information</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/main-menu?" target="_blank">Use the Main menu to start an activity</a>|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/make-calls-directly-dynamics-365-guides-hololens-app" target="_blank">Make calls directly (Preview) from Dynamics 365 Guides</a>| Yes |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/make-call" target="_blank">Make a call (Preview) in the Dynamics 365 Guides HoloLens app</a>|
| <a href="https://docs.microsoft.com/dynamics365-release-plan/2021wave2/guides/dynamics365-guides/planned-features" target="_blank">Ability to create very long guides</a>| No |<a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/hololens-app-place-holograms" target="_blank">Place and manipulate holograms in the Dynamics 365 Guides HoloLens app</a>|

> [!NOTE]
> If you have created any custom security roles, make sure to update those custom roles to match the permissions for relevant Dynamics 365 Guides Security roles (Author, Operator, Restricted Author, Restricted Operator) so that any custom roles have access to the new MR App Session table.

### Bugs fixed and other improvements

- Improved PC app stability around step deletion
- Fixed unsupported scenario that allowed users to specify a trigger style

> [!TIP]
> Looking for a list of earlier features? Go to <a href="https://docs.microsoft.com/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>.

## See also

- <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>

- <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a>

- <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">Check compatibility between the Dynamics 365 Guides Dataverse solution and PC/HoloLens apps</a>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
