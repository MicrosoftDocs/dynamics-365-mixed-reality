---
author: Mamaylya
description: Describes the new features in Dynamics 365 Guides, organized by release date.
ms.author: mamaylya
ms.date: 12/5/2022
ms.topic: reference
title: What's new in Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# What's new in Dynamics 365 Guides

This page provides details about the **current wave of features (October 2022 through March 2023)** for [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], organized by release date. To see a comprehensive list of released and upcoming features, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>. You can also <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">see a complete list of features organized by previous waves</a>. 

> [!IMPORTANT]
> Guides Dataverse solution version 800.0.0.1, which is now available, is a foundational change for key features in upcoming Dynamics 365 Guides releases and includes the new PhoneCall table. Updated versions of the PC and HoloLens apps are available for the new solution and **require the 800.0.0.1 or newer solution.** Also, if you have created any custom security roles, **make sure to update those custom roles to match the permissions for relevant Dynamics 365 Guides Security roles (Author, Restricted Author) so that any custom roles have access to the PhoneCall table. In the Power Apps Security Role dialog box, this is the Activity table. Users with custom roles derived from the Author or Restricted Author security roles will be unable to log into the HoloLens and PC apps until the custom security roles are updated.**  
> 
> If you choose not to update the solution and remain on the version 700 solution and compatible versions of the PC and HoloLens apps, there's no impact.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md). See the **Features** table below to determine if a new feature requires a solution update. 

If you have feature requests or suggested improvements, send them to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] team at <a href="https://aka.ms/GuidesIdeas" target="_blank" data-linktype="absolute-path">https://aka.ms/GuidesIdeas</a>.

## December 6, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app||
|HoloLens app (HoloLens 2 only)||
|Solution||

### Bugs fixed and other improvements

- Fixed an issue where video toggle and recording buttons might have been unavailable in certain conditions on Hololens 2
- Fixed an issue with calling indicator not updating after recording had finished on Hololens 2
- Improved behavior of automatic video switching while in a call on Hololens 2
- Improved reliability of displaying screen shared by other participants while in a call/meeting on Hololens 2
- Improved reliability of displaying participants that are currently speaking in a call/meeting in addition to some visual issues on Hololens 2
- Improved app performance and optimized memory usage on Hololens 2
- Extended Voice Command support through menus
- Fixed issue with multiple slates highlighting when gazing

## Earlier releases

Looking for a list of features from earlier releases? Go to <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>.

## See also

- <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>

- <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a>

- <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">Check compatibility between the Dynamics 365 Guides Dataverse solution and PC/HoloLens apps</a>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
