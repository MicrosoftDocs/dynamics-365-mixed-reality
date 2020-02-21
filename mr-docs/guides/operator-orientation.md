---
author: Mamaylya
description: Learn how to operate a guide in Microsoft Dynamics 365 Guides by using the HoloLens app.
ms.author: mamaylya
ms.date: 02/25/2020
ms.service: crm-online
ms.topic: article
title: Operate a guide in Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Operate a guide in Dynamics 365 Guides

<!--
![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about operating a guide](https://aka.ms/guidesoperate)
-->

When you open a guide as an operator by using the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] HoloLens app, you will see the Step card. The Step card is the hub of everything that you do in a guide. It provides the instructions that you follow to complete a task. It also includes two buttons that you use to navigate through a guide: **Next Step** and **Go Back**. As you go through the steps in a task, the Step card follows you on [!include[pn-hololens](../includes/pn-hololens.md)], to keep the instructions where you need them.

![Step card with Next Step and Go Back buttons](media/pin.PNG "Step card with Next Step and Go Back buttons")

## Get oriented with the Step card

In addition to the **Next Step** and **Go Back** buttons, the Step card includes several buttons and user interface (UI) elements that help you perform various actions.

![Step card buttons](media/operator-step-card-orientation.PNG "Step card buttons")

Here is a description of the buttons and other UI elements on the Step card.

| Number | UI element | Name | Purpose |
|---|---|---|---|
| 1 | ![Home button](media/home-button.png "Home button") | Home | Select a different guide. |
| 2 | ![Follow mode button](media/follow-button.png "Follow mode button") | Follow mode | Have the Step card follow you around, or lock it to a location.<p>If you turn off **Follow** mode, the Step card stays where it is. You can move the Step card wherever you want at any time. Just grab it by using the navigation bar. For more information, see the "Follow and pinning" section later in this topic.</p> |
| 3 | ![Anchor button](media/anchor-button.PNG "Anchor button") | Anchor button | Re-anchor (realign) the guide.<p>[!include[pn-hololens](../includes/pn-hololens.md)] can sometimes lose tracking, which causes holograms to become misaligned. To fix this issue, you must re-anchor the guide by gazing at the anchor again. For more information, see the [Anchor your guide](operator-anchor.md).</p> |
| 4 | ![Settings button](media/settings-button.png "Settings button") | Settings | See the build of [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] that you're using. |
| 5 | ![Profile button](media/profile-button.png "Profile button") | Profile | Sign in and out. |
| 6 | ![Step progress](media/step-progress.PNG "Step progress") | Step progress | See where you are in the step. |
| 7 | ![Outline button](media/outline-button.png "Outline button") | Outline | Go to the **Outline** page.<p>You can use the **Outline** page to quickly move around your guide. The following illustration shows the **Outline** page for a Pylon wiring guide.</p><p>![Outline page](media/outline-operator.PNG "Outline page")</p> |
| 8 | ![Task name](media/task-name-table.PNG "Task name") | Task name | See the name of the task that you're working on. |
| 9 | ![Task progress](media/task-progress.PNG "Task progress") | Task progress | See where you are in the task. |

## Use a dotted line to help you find the focus area for a step

Step cards are linked by holographic dotted lines to physical areas in your work area. These dotted lines help you find the area where you must take action.

![Holographic dotted line](media/dotted-line.PNG "Holographic dotted line")

### Dotted line tips and tricks

- Follow the dotted line to find the physical area where you must do the work. Follow the dotted line back to the Step card to read the instructions.

- If the dotted line points behind you, step to the side, and then continue to follow it.

- Note that the dotted line might sometimes go through real-world objects.

## Use Follow mode and pinning

You will notice that, wherever you look, the Step card follows your gaze. Therefore, while you're working, you never have to worry about where your instructions are. You can stop the Step card from following you by turning off **Follow** mode from the navigation bar.

![Follow mode button](media/follow-button-nav-bar.PNG "Follow mode button")

You can also grab the navigation bar at any time to place the card where you want it.

![Grabbing the navigation bar](media/follow-button-move-card.PNG "Grabbing the navigation bar")

## Access a website that's linked from the Step card

If a Step card includes a **Website link** button, you can go to the website by selecting the button. For example, there might be a link to a parts diagram or a parts inventory system. The website is opened in the HoloLens Edge browser. When you close the browser, you go back to the step that you were working on.

![Website link button](media/website-button-runtime.PNG "Website link button")

## Launch an app created in Power Apps from the Step card

If a Step card includes a **Power Apps** button, you can launch an app by selecting the button. The app opens in a browser on HoloLens. When you close the browser, you return to the step. 

>[!NOTE]
>You need a Power Apps license to run Power Apps from Dynamics 365 Guides. You must also have permission to view the app created in Power Apps.

![PowerApps button](media/website-button-runtime.PNG "PowerApps button")

## Turn off holograms

If you ever feel that holograms are getting in the way, you can turn them off with a glance. (You can also turn them back on.) To turn off a hologram, gaze at the eye symbol in the middle of the dotted line.

![Eye symbol](media/dotted-line-toggle-visibility.PNG "Eye symbol")

## See also

<!--![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video about operating a guide](https://aka.ms/guidesoperate)<br>
-->
![Doc graphic](media/doc-icon.PNG "Doc graphic") [Calibrate your HoloLens](https://docs.microsoft.com/windows/mixed-reality/calibration)
