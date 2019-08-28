---
author: drpusey
description: Dynamics 365 Remote Assist mobile app user guide
ms.author: drpusey
ms.date: 06/07/2019
ms.service: crm-online
ms.topic: article
title: Dynamics 365 Remote Assist mobile app user guide
ms.reviewer: v-brycho
---

# Dynamics 365 Remote Assist Mobile user guide (in preview)

[This topic is pre-release documentation and is subject to change.]

The [!include[cc-microsoft](../../includes/cc-microsoft.md)] [!include[pn-dyn-365-remote-assist](../../includes/pn-dyn-365-remote-assist.md)] mobile app extends the capabilities of [!include[pn-dyn-365-remote-assist](../../includes/pn-dyn-365-remote-assist.md)] to work with [!include[tn-android](../../includes/tn-android.md)] 
ARCore-capable phones (in addition to [!include[cc-microsoft](../../includes/cc-microsoft.md)]  [!include[pn-HoloLens](../../includes/pn-HoloLens.md)]). Technicians can use their phones to connect and collaborate with an 
expert on [!include[pn-microsoft-teams](../../includes/pn-microsoft-teams.md)]. Using live video calling and mixed reality annotations, they can share what they see with the expert 
to troubleshoot problems together, faster. 

## What you’ll need

You’ll need the following to use the [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] mobile app:

- An [!include[tn-android](../../includes/tn-android.md)] ARCore-capable phone (tablets are not currently supported), with ARCore installed. [View the full list of supported 
devices.](https://developers.google.com/ar/discover/supported-devices) 

- A [!include[tn-google](../../includes/tn-google.md)] Play account.

- The [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] mobile app.

- A [!include[pn-microsoft-teams](../../includes/pn-microsoft-teams.md)] account (available for free).

- A [!include[pn-microsoft-teams](../../includes/pn-microsoft-teams.md)] desktop client running [!include[pn-ms-windows-short](../../includes/pn-ms-windows-short.md)] 10 (for the remote expert receiving the call).

- An internet connection. At least 1.5 MB of bandwidth is recommended for the best experience.

If you want to use [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] together with [!include[pn-dyn-365-field-service](../../includes/pn-dyn-365-field-service.md)] so you can automatically log call information to a 
[!include[pn-field-service](../../includes/pn-field-service.md)] work order, you’ll also need one or both of the following:

- [!include[pn-dyn-365-field-service](../../includes/pn-dyn-365-field-service.md)] web application

- [!include[pn-dyn-365-field-service](../../includes/pn-dyn-365-field-service.md)] mobile app 

## Get started

### Step 1: Sign up for a Microsoft Teams account (free)

A [!include[pn-microsoft-teams](../../includes/pn-microsoft-teams.md)] account is required to use [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] mobile. If you don’t already have a [!include[pn-teams](../../includes/pn-teams.md)] account, you can [create a Teams account for free](https://businessstore.microsoft.com/en-us/create-account/signup?products=CFQ7TTC0K8P5:0001&lm=deeplink&lmsrc=freePageWeb&cmpid=FreemiumSignUpHeader). 

### Step 2: Download the app

1.	Go to the [!include[tn-google](../../includes/tn-google.md)] Play Store: https://play.google.com/store/apps/details?id=com.microsoft.ramobile.

2.	Select **Download**. 
 
### Step 3: Sign in to the app for the first time

1.	After you’ve downloaded the app, open it on your [!include[tn-android](../../includes/tn-android.md)] phone. 

2.	Sign in with your [!include[pn-microsoft-teams](../../includes/pn-microsoft-teams.md)] account.

    ![Sign-in screen](../media/sign-in.png "Sign-in screen")
  
    > [!TIP]
    > The sign-in address will be in the form: username@company.
    
3.	In the dialog box that appears, select **Enable Feature** to link [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] to [!include[pn-dyn-365-field-service](../../includes/pn-dyn-365-field-service.md)], or 
select **Skip** if you don’t want to link the apps at this time. You can always link them later through **Settings**. To learn more about how the apps work together, select **Learn More**.

    ![Field Service screen](../media/field-service.PNG "Field Service screen")
  
## Make a call
After signing in, you’ll see the **Contacts** page, which is the main page in the [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] mobile app. On the **Contacts** page, 
your contacts are organized by the most recent calls.

![Contacts screen](../media/contacts.PNG "Contacts screen")


To make a call:

1.	Select ![Search button](../media/search-icon.PNG "Search button"), enter the name of the contact to search for, and then select the contact from the resulting list.
       
    ![Search for a contact](../media/search-contact.PNG "Search for a contact")
    
2.	In the contact card, select **Launch Call**.

    ![Launch Call screen](../media/launch-call.PNG "Launch Call screen")
  
    Use the buttons in the bar at the bottom of the screen to mute the call, pause the video feed, turn on the speaker phone, or 
    end the call.
    
    ![Call controls](../media/call-controls.PNG "Call controls")
  
 
## Add annotations
You can add annotations to your screen to share with an expert on the call. To create annotations, your phone needs to recognize 
at least one plane (vertical or horizontal) in your work area. You do this by scanning your work area with the phone. When a plane has been recognized, you’ll see a confirmation visualization and the annotation toolbar will appear at the top of the screen:

![Add annotations](../media/annotation-bar-full-screen.PNG "Add annotations")
  
> [!NOTE] 
> If you lock your phone or minimize [!include[pn-remote-assist](../../includes/pn-remote-assist.md)], the recognized planes will reappear automatically as soon as your phone recognizes the environment.

### Add an annotation
You can add an annotation by using the buttons on the annotation toolbar:

![Annotation bar](../media/annotation-bar.PNG "Annotation bar")
  
For example, to add an arrow, tap the arrow tool and drag your finger to the spot where you want to place the arrow.

### Minimize or restore the toolbar

To minimize the toolbar if you want to see more of the screen:

- Select the arrow on the right side of the toolbar. 

  ![Minimize bar](../media/minimize-bar.PNG "Minimize bar")
 
To restore the toolbar to its original size:

- Select the **Pen** button. 

  ![Pen button](../media/pen-button.PNG "Pen button")

### Make the expert’s video feed bigger

When you call an expert, the expert’s video feed appears in the lower-right corner of your phone screen. To make the expert’s 
video feed bigger, tap the feed. Tap the feed again to return to the original size.

![Expert video feed](../media/expert-annotating.PNG "Expert video feed")
  
If the expert is annotating, a notification icon will appear on the expert's feed.  

## Switch the camera view from portrait to landscape

You can switch the orientation of the camera view from portrait to landscape while in a call by changing the orientation of your phone. Using landscape view provides a wider field of view, which may improve the experience for the remote expert on the call.
   
## Use Remote Assist together with Dynamics 365 for Field Service

You can use [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] together with [!include[pn-dyn-365-field-service](../../includes/pn-dyn-365-field-service.md)] if you want to automatically log call information to a 
[!include[pn-field-service](../../includes/pn-field-service.md)] work order when you end the call. 

When you sign in to the [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] mobile app for the first time, you’re prompted to link [!include[pn-remote-assist](../../includes/pn-remote-assist.md)] to [!include[pn-dyn-365-field-service](../../includes/pn-dyn-365-field-service.md)]. You can link the apps through **Settings** if you chose not to link them at first sign-in.

### Link the Remote Assist mobile app to Dynamics 365 for Field Service

1.	Select the **Main menu** ![Main menu button](../media/main-menu-button.PNG "Main menu button") button.

2.  Select the **Settings** button.  

3.	In the **Settings** dialog box, move the slider to on.

    ![Settings screen](../media/settings.PNG "Settings screen")
  
### Save call data to a Field Service work order

1.	When you end the call, the following dialog box will appear:

    ![Post to Work Order screen](../media/post-to-work-order.PNG "Post to Work Order screen")
  
2.	Select **Post**.

3.	In the **Select a Booking** screen, select the appropriate booking to post the call data to.

    ![Select a Booking screen](../media/bookings-today.PNG "Select a Booking screen")
  
    > [!NOTE]
    > If you don’t see the booking you’re looking for, it might be because you have access to multiple instances (organizations). 
    To switch to a different instance, select the ellipsis button (...), and then select the instance you want.<br>![Select instance](../media/select-instance.PNG "Select instance")
    
## Sign out of the app

1.	Select the **Main menu** ![Main menu button](../media/main-menu-button.PNG "Main menu button") button.

2.	Select **Sign Out**.

## Get Help

1.	Select the **Main menu** ![Main menu button](../media/main-menu-button.PNG "Main menu button") button.

2.	Select **Help**.

## Get support or provide feedback

If you’d like to get direct access to the product team forum and provide feedback on the mobile app preview:

1.	Sign up for the [!include[pn-dyn-365-remote-assist](../../includes/pn-dyn-365-remote-assist.md)] Mobile Public Preview Insiders Program at https://experience.dynamics.com. 


2.	Select the **Insider Program** box, which will lead you to the Insider Program application.

    ![Insider Program button](../media/insiders-program.PNG "Insider Program button")
 
You can also provide feedback directly from the app by using the following procedure:

1.	Select the **Main menu** ![Main menu button](../media/main-menu-button.PNG "Main menu button") button.

2.	Select **Feedback**.

### See also

[Troubleshoot Dynamics 365 for Field Service integration with Remote Assist](../troubleshoot-field-service.md)
