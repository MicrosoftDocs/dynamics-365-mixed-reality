---
title: 
description: 
ms.date: 03/09/2023
ms.topic: 
ms.service: 
author: 
ms.author: 
manager: 
---

# Anchor guides content through QR codes and embed deep links 

As an instructional tool, the attractiveness and effectiveness of guides partly stem from the use of 3D content such as arrows to nudge end-users' attention towards specific points of interest on machinery.

 

To create a successful and safe guide, the author will not only need to follow [<u>3D object best practices</u>](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/hololens-app-place-holograms#best-practices-for-working-with-3d-content) when authoring instructions, your organization also needs to choose a way for Guides to continuously place holograms correctly in physical space, i.e., where the author intended a hologram to appear in relation to machinery. 

If a 3D arrow, for instance, indicates that the end-user must connect a wire to socket three out of five neighboring sockets, all stakeholders in your organization want to ensure an accurate placement of the hologram. Otherwise, you risk misguiding the operator and potentially cause an incorrect, potentially dangerous, assembly or operation of equipment.  

  

The placing of 3D objects in space is achieved through one of [<u>four available anchoring methods</u>](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/pc-app-anchor#four-ways-to-anchor-a-guide): Azure Object Anchors (in preview), QR code anchor, circular code anchor, and holographic anchor.

For Guides usage in a regulated setting, the [<u>QR code anchor</u>](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/pc-app-anchor-qr-code) is the recommended anchoring method. When using this method, guides will be launched by scanning a digital or printed QR code through the HoloLens, and all 3D elements will be positioned in the production area with the QR code representing point zero in X Y Z axis.

It is recommended to generate a unique QR code for each station, equipment etc. that has an associated guide and [<u>embed a deep link</u>](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/pc-app-anchor-embed-qr-code-link) in each QR code to a unique, validated, guide existing in an Execution environment. This will assist you in being compliant with your organization's quality management processes because only approved and specific guides will be launchable on location.

Without deep links embedded, operators will be presented with an overview of selectable guides from the Execution environment with the risk of selecting the wrong guide. Particularly, this poses a risk, if you have machinery with similar instructions, or have multiple guides for the same machinery, for instance in relation to switching settings.

When working with QR code anchors at a production site, best practices regarding [<u>printing settings, size, location, orientation, and contrast</u>](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/pc-app-anchor-qr-code#best-practices-for-qr-code-anchors) will help you succeed with anchoring and expedite QA validation of your guides. However, your industry's specific requirements might collide with these anchor best practices: you might be forced to compromise with best practices to stay compliant. For example, your organization requires laminated QR codes in a lab setting, even though glossy materials can negatively affect scanning due to reflected light.


