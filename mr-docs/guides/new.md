---
author: Mamaylya
description: Describes the new features in Dynamics 365 Guides, organized by release date.
ms.author: mamaylya
ms.date: 12/8/2022
ms.topic: reference
title: What's new in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# What's new in Dynamics 365 Guides

This page provides details about the **current wave of features (October 2022 through March 2023)** for [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], organized by release date. To see a comprehensive list of released and upcoming features, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>. You can also <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">see a complete list of features organized by previous waves</a>.

If you have feature requests or suggested improvements, send them to the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] team at <a href="https://aka.ms/GuidesIdeas" target="_blank" data-linktype="absolute-path">https://aka.ms/GuidesIdeas</a>.

## December 8, 2022

|Item|Version|
|-------------------------|--------------------------------|
|PC app|801.2212.2001.0 |
|HoloLens app (HoloLens 2 only)|801.2212.2001.0 |
|Solution|800.1.0.1 |

> [!NOTE]
> Version 801.2212.2001.0 needs Dynamics 365 Guides solution version 800.0.0.1 or later. If you choose not to update your PC and HoloLens apps and the Dynamics 365 Guides solution, there's no impact and you can continue to use Dynamics 365 Guides with the existing feature set. To update your solution, see <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Update the Dynamics 365 Guides solution</a>. For more information about solution and app compatibility, see [Compatibility between Dynamics 365 Guides solution and apps](admin-apps-solution-compatibility.md).

### Bugs fixed and other improvements

This release fixes image quality issues for textures on 3D content and slate images. Highly detailed 2D and 3D content textures, especially those with linear patterns, now have restored clarity on the HoloLens. This change may increase memory requirements and cause new warnings or content loading issues if existing steps already exceed or nearly exceed recommended limits. Customers experiencing memory issues should review [Optimize your 3D models to use with Dynamics 365 Guides and Power Apps](/3d-content-guidelines/optimize-models.md) and [Best practices for converting and optimizing real-time 3D models for use in Dynamics 365 mixed-reality apps](/3d-content-guidelines/best-practices.md).

**Calling**
- Fixed issue where video toggle and recording buttons might have been disabled
- Fixed issue where the call recording indicator wouldn’t show correct state
- Improved behavior of automatic video switching while in a call
- Improved reliability of displaying screen shared by other participants while in a call/meeting
- Improved reliability of displaying participants that are currently speaking in a call/meeting and fixed some visual issues

**Slates**
- Fixed EXIF images that displayed incorrectly on slates 
- Fixed aspect ratio sizing when screen sharing
- Fixed cursor visibility on slates in authoring mode
- Improved sound FX when interacting with slates
- Added titles to images opened from a chat
- Fixed cursor to remain at the grab position when moving slates
- Fixed issue with multiple slates highlighting when gazing at a single slate

**File browsing**
- Fixed inconsistencies in the UI including button and breadcrumb positions
- Fixed issue with file usage when internet connectivity is lost and recovered

**Object anchors**
- Fixed issue that prevented object anchor creation
- Fixed issue that prevented object anchor detection on similar looking shapes

**Other**
- Removed preview indicator on the **Settings** page of the mobile-driven app for calling capabilities
- Improved media player stability on PC app

## Earlier releases

Looking for a list of features from earlier releases? Go to <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>.

## See also

- <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>

- <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a>

- <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">Check compatibility between the Dynamics 365 Guides Dataverse solution and PC/HoloLens apps</a>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
