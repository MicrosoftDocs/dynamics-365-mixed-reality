---
author: prashantyvr
description: Overview of authoring in Dynamics 365 Guides, including PC authoring and HoloLens authoring
ms.author: prashan
ms.date: 08/10/2023
ms.topic: overview
title: Authoring with the PC app and HoloLens app in Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Overview of authoring a guide in Dynamics 365 Guides
 
[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

To author a guide in Microsoft Dynamics 365 Guides, you use two apps:

- **PC app.** You start with the PC application. Use this application to create the guide, choose an anchoring method, add tasks and steps, write the instructions for your steps, and assign different types of assets to support those steps. Supporting assets include:

  - Your custom 3D objects.

  - 3D objects from the toolkit, a library of predefined objects included in Guides such as arrows and numbers.

  - 2D media (images and videos).

- **HoloLens app.** After creating the guide with the PC app, use the HoloLens app in Author mode to test the flow of your guide, place your holograms in the real world, add holographic dotted lines to show operators where to focus, and add styles for 3D objects (warning or caution, for example).

    > [!TIP]
    > You can use both apps to edit the same guide simultaneously for the fastest workflow. Create the structure and text in the PC app, do the 3D placement in the HoloLens app, and then work back and forth until you have your guide just the way you want it.

  ![Authoring overview.](media/authoring-overview.PNG "Authoring overview")
  
  [!INCLUDE [add-guest-user.md](../includes/add-guest-user.md)]

## How the PC app and HoloLens app work together

When you edit a guide at the same time in the PC and HoloLens apps, Autosave synchronizes your changes across both apps. Edits are automatically saved and synced to the server every few seconds. You can also select **Save** at any time. The apps refresh automatically when they detect any changes made to the guide from another device.

After you're done editing, we recommend pausing for a couple seconds before closing the app to make sure the app has time to sync with the server.

In the HoloLens application, if you leave the app, it goes on standby (doesn't close). When you select the app tile, you'll return to where you were before, and no changes are lost.

### Guide out of sync...refreshing

This message indicates you and another user are editing the same guide on separate devices. The guide is automatically saved on the other device first, then updated on the server. When the current device learns of the update, it reloads the latest version of the guide from the server.

## How do I stream my HoloLens view to a PC using Miracast?

The Connect app for wireless projection using Miracast is no longer installed by default on the PC, but is available as an optional feature. To add the feature on the PC, select **Settings** > **System** > **Optional features** > **Add a feature**, and then add the Wireless Display feature. 

The Connect app is automatically installed by default on the HoloLens. To initiate sharing from the HoloLens:

From the OS start menu, select **Cast screen** :::image type="icon" source="media/hololens-cast-screen.png":::.

## Next steps

- ![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about PC authoring](https://aka.ms/pcauthor)

- ![Doc graphic](media/doc-icon.PNG "Doc graphic") [Overview of authoring a guide with the PC app](pc-app-overview.md)

- ![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about HoloLens authoring (shows HoloLens 1 version)](https://aka.ms/hololensauthor)

- ![Doc graphic](media/doc-icon.PNG "Doc graphic") [Overview of authoring a guide with the HoloLens app](hololens-app-overview.md)
- ![Doc graphic](media/doc-icon.PNG "Doc graphic") [Gestures for authoring and navigating](authoring-gestures-HL2.md)
- ![Doc graphic](media/doc-icon.PNG "Doc graphic") [How to make a great guide](great-guide.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
