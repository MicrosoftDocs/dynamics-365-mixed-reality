---
author: Mamaylya
description: Learn about how HoloLens (first gen) works with and Dynamics 365 Guides
ms.author: davepinch
ms.date: 11/08/2021
ms.topic: article
title: Use HoloLens (first gen) devices with Dynamics 365 Guides
ms.reviewer: v-wendysmith
---

# Use HoloLens (1st gen) devices with Dynamics 365 Guides

HoloLens (1st gen) has entered Long-Term Servicing State for Dynamics 365 Guides and is no longer supported for the latest versions of Dynamics 365 Guides. This article accumulates all documentation related to using HoloLens (1st gen) devices. Customers on HoloLens (1st gen) can continue using the last supported app version (600.2103.19001) released on April 1, 2021. This version of the app is compatible with all 500 solution versions up to and including 600.0.0.1, also released on April 1, 2021. To continue using HoloLens (1st gen), existing customers should not upgrade to a solution version later than 600.0.0.1. Solution version 600.0.0.1 is no longer available for download for new HoloLens 1 customers.

## Gestures for authoring and navigating in Dynamics 365 Guides 

To author and navigate through a guide in [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)], you'll use gaze and a few gestures.

### Gaze
The easiest way to get around a guide is to gaze at an item (menu or button, for example). If the item has a selection box or circle (gaze/dwell button), you can select the item just by gazing at the button hit zone. The item is selected when the box or circle is filled. 

![Gaze gesture.](media/gaze-fill-2.gif "Gaze gesture")
 
In other cases, you use gaze to target an item, and then act on that selection by using a gesture. When you gaze, turn your whole head—not just your eyes. The cursor will follow. 

### Gestures
This section lists the most important gestures to know when working with [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)].

#### Bloom 
The bloom gesture opens the **Start** menu or the **Quick Actions** menu, depending on which version of HoloLens you're using. Most of the time, you only need to use the bloom gesture once to get to **Start**, but sometimes you'll need to use it twice. If you're not sure what to do at any time, the bloom gesture is a good way to get reoriented. 

To do the bloom gesture: 
1.	Hold out your hand with your palm up and your fingertips together. 
2.	Open your hand.

![Bloom gesture.](media/bloom-gesture.PNG "Bloom gesture")
 
#### Air tap
Use air tap, along with gaze, to select holograms and any gaze/dwell buttons. To do an air tap:
1.	Gaze at a hologram.
2.	Hold your hand straight out in front of you in a loose fist, then point your index finger straight up toward the ceiling. You don't need to raise your whole arm—keep your elbow low and comfortable.
3.	Tap your finger down, then quickly raise it back up again.

![Air tap gesture.](media/air-tap-gesture.PNG "Authoring overview")
 
#### Air tap and hold
Use air tap and hold to move, rotate, or scale holograms when authoring. To air tap and hold, start with an air tap, but keep your finger down instead of raising it back up again. 

#### The gesture frame
[!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-hololens](../includes/pn-hololens.md)] has sensors that can see a few feet to either side of you. When you use gestures, you need to keep them inside that frame, or [!include[pn-hololens](../includes/pn-hololens.md)] won't see them. As you move around, the frame moves with you. When your hand is inside the frame, the cursor looks like a ring. When [!include[pn-hololens](../includes/pn-hololens.md)] can't see your hand, the cursor changes to a dot.

### Need a tutorial on gestures?
For a tutorial on some basic gestures, close [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] by blooming and selecting **Mixed Reality Home**, use the bloom gesture to go to **Start**, and then select **Learn Gestures**. If you're having trouble with gestures, see [HoloLens and holograms: FAQ](https://support.microsoft.com/help/13456/hololens-and-holograms-faq).

## Calibrate your HoloLens 1 device

1. Use the bloom gesture to open the **Start** menu.

2. Air tap **Calibration**.

    ![Calibration button.](media/hololens-calibration.PNG "Calibration button")

3. Follow the instructions on your [!include[pn-hololens](../includes/pn-hololens.md)].

All users must do this calibration after they sign in to the device. If HoloLens is running Windows Holographic for Business edition, the IPD settings are saved on the device. When you sign in to the same HoloLens, your IPD settings are automatically applied, even after you switch users; you don't have to recalibrate the device. However, if HoloLens is running Windows Holographic edition, user settings aren't saved because this version of the operating system is designed for a single user. So you must recalibrate the device whenever you switch users.

To determine which version of the operating system you're using on [!include[pn-hololens](../includes/pn-hololens.md)], follow these steps.

1. Use the bloom gesture to open the **Start** menu.

2. Air tap **Settings \> System**.

3. Air tap **About**.
