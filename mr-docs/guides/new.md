---
author: davepinch
description: Describes the new features in Dynamics 365 Guides, organized by release date.
ms.author: davepinch
ms.date: 03/06/2024
ms.topic: conceptual
title: What's new in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

<br />
<!--Keep line break for proper in-app rendering!-->
<!---All links must be in "a hrefs" in order for this page to render correctly in the app!-->

# What's new in Dynamics 365 Guides

This page provides details about the latest release in the **current wave of features (October 2023 through March 2024)** for Microsoft Dynamics 365 Guides, organized by release date. To see a comprehensive list of released and upcoming features, see <a href="/dynamics365/release-plans/" target="_blank">Dynamics 365 and Power Platform release plans</a>. You can also <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">see a complete list of features organized by previous waves</a>.

If you have feature requests or suggested improvements, send them to the Dynamics 365 Guides team at <a href="https://aka.ms/GuidesIdeas" target="_blank">https://aka.ms/GuidesIdeas</a>.

## March 11, 2024

|Item|Version|
|-------------------------|--------------------------------|
|PC app| 903.x  |
|HoloLens app | 903.x  |
|Solution|  900.3.x  |

### Feature

- Completion steps can now have a <a href="/dynamics365/mixed-reality/guides/pc-app-website-powerapps-link" target="blank">link to a website, email, guide, custom app, or Power Apps</a>. Operators can complete a guide and easily navigate to another custom resource or continue through their workflow.

## February 27, 2024

|Item|Version|
|-------------------------|--------------------------------|
|PC app| 902.2402.16001.0  |
|HoloLens app | 902.2402.16001.0  |
|Solution|  900.2.0.4  |

### Bugs fixed and other improvements

- A new copy API allows developers to programmatically make a copy of a guide in the same environment.
- <a href="/dynamics365/mixed-reality/guides/pc-app-add-3D-part" target="blank">3D object complexity statistics</a> appear on the object's **Properties** tab in the PC app and a warning displays if a 3D object exceeds the recommended complexity limits.
- Performance improvements on HoloLens when loading objects in Guides steps.
- Calls now end when the Guides app is closed or minimized on HoloLens. To keep calls active, disable the <a href="/dynamics365/mixed-reality/guides/change-setting" target="blank">End calls on suspend setting</a> on the HoloLens.

## December 20, 2023

|Item|Version|
|-------------------------|--------------------------------|
|PC app| 901.2312.16001.0 |
|HoloLens app (HoloLens 2 only)| 901.2311.28001.0 |
|Solution| 900.1.0.0 |

Version 901.2312.16001.0 fixes an issue in the PC app where the app stops responding if you use a non-English language and select the **All** or **Recent** tab.

> [!IMPORTANT]
> Guides 901.x isn't compatible with Guides 800 solutions. If you choose not to update to the 900 solution and remain on the version 800 solution and compatible versions of the PC and HoloLens apps, *don't* update to the 901.x version.
>
> If you updated to the Guides Dataverse solution version 900.0.1.1, update the PC app version.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md).

## December 05, 2023

|Item|Version|
|-------------------------|--------------------------------|
|PC app| 901.2311.28001.0 |
|HoloLens app (HoloLens 2 only)| 901.2311.28001.0 |
|Solution| 900.1.0.0 |

### Bugs fixed and other improvements

- <a href="/dynamics365/mixed-reality/guides/calling-photos" target="blank">Take a photo within Guides</a> through the HoloLens and share it with other call participants</a>.
- Guides dynamically manages loaded content in response to overall system memory usage. This improves device stability when using multiple HoloLens features simultaneously (such as Guides, calling, files, mixed reality capture (MRC), and Edge browser) and allows more file content to display. However, when multiple features are in use at once, anticipate potentially longer loading times when navigating through a guide.
- Guides limits the maximum size of a single texture on a 3D object to 16 megapixels (such as 4K x 4K or equivalent).

> [!IMPORTANT]
> Guides 901.x isn't compatible with Guides 800 solutions. If you choose not to update to the 900 solution and remain on the version 800 solution and compatible versions of the PC and HoloLens apps, *don't* update to the 901.x version.
>
> If you updated to the Guides Dataverse solution version 900.0.1.1, update to the new solution and PC and HoloLens app versions.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md).

## November 06, 2023

|Item|Version|
|-------------------------|--------------------------------|
|PC app| 900.2311.2001.0 |
|HoloLens app (HoloLens 2 only)| 900.2311.2001.0  |
|Solution| 900.0.1.1 |

Version 900.2311.2001.0 fixes a performance issue in the PC and HoloLens apps.

> [!IMPORTANT]
> If you updated to the Guides Dataverse solution version 900.0.1.1, you just need to update to the new  PC and HoloLens apps versions. If you chose not to update to the 900 solution and remain on the 800 version solution and compatible versions of the PC and HoloLens apps, there's no impact.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md).

## November 01, 2023

|Item|Version|
|-------------------------|--------------------------------|
|Solution| 900.0.1.1 |

This solution version includes minor fixes and improvements.

> [!IMPORTANT]
> If you updated to the Guides Dataverse solution version 900.0.0.1 and updated the PC and HoloLens apps, you just need to update to the new 900.0.1.1 solution. If you chose not to update to the 900 solution and remain on the 800 version solution and compatible versions of the PC and HoloLens apps, there's no impact.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md).

## October 17, 2023

|Item|Version|
|-------------------------|--------------------------------|
|PC app| 900.2130.7001.0 |
|HoloLens app (HoloLens 2 only)| 900.2130.7001.0 |
|Solution| 900.0.0.1 |

> [!IMPORTANT]
> Guides Dataverse solution version 900.0.0.1 is a mandatory update for key features in upcoming Dynamics 365 Guides releases. To update to the 900 solution, update the solution and the PC and HoloLens apps. Guides 901.x, scheduled to be released in December 2023, won't be compatible with Guides 800 solutions. If you choose not to update to the 900 solution and remain on the version 800 solution and compatible versions of the PC and HoloLens apps, there's no impact.
>
> Work with your IT admin to schedule installation updates or <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">see instructions for updating the solution</a>. You can also [learn more about which solutions work with which applications](admin-apps-solution-compatibility.md).

### Bugs fixed and other improvements

- For organizations with multiple environments, quickly <a href="/dynamics365/mixed-reality/guides/switch-environment" target="blank">switch environments.</a>
- <a href="/dynamics365/mixed-reality/guides/package-a-guide" target="blank">Package a guide</a> to create a self-contained, read-only file.
- <a href="/dynamics365/mixed-reality/guides/pc-app-anchor-azure-object" target="blank">Anchor guides with object anchors</a> is generally available (GA).
- Fixed an issue where Teams mobile users couldn't view or download photos shared by HoloLens users

## Earlier releases

Looking for a list of features from earlier releases? Go to <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>.

## See also

- <a href="/dynamics365/mixed-reality/guides/version-history" target="_blank">Version history for Dynamics 365 Guides</a>

- <a href="/dynamics365/mixed-reality/guides/upgrade" target="_blank">Upgrade your Dynamics 365 Guides solution</a>

- <a href="/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility" target="_blank">Check compatibility between the Dynamics 365 Guides Dataverse solution and PC/HoloLens apps</a>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
