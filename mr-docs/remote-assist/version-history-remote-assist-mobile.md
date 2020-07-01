---
title: "Remote Assist mobile version history | MicrosoftDocs"
ms.custom: 
  - dyn365-mixed-reality-remote-assist
ms.date: 07/01/2020
ms.reviewer: krbjoran
ms.service: dynamics-365-mixed-reality-remote-assist
ms.suite: ""
ms.technology: 
  - "remote-assist"
ms.tgt_pltfrm: ""
ms.topic: "article"
applies_to: 
  - "Dynamics 365 (online)"
  - "Dynamics 365 Version 9.x"
author: FieldServiceDave
ms.assetid: f7e513fc-047f-4a88-ab83-76fae5e583e2
caps.latest.revision: 42
ms.author: daclar
manager: shellyha
search.audienceType: 
  - admin
  - customizer
search.app: 
  - MRRA
  - MRRA
---

# Remote Assist mobile version history

## iOS - 2020.7.1 + Android - 2020.06.27

Date: July 1, 2020

-	Improved incoming call experience for Remote Assist mobile users who do not have the app open when a call comes in from Microsoft Teams desktop or mobile clients.
-	Fix for app crashing on mobile devices without augmented reality (AR) support, especially iPhone 5 and iPhone 6 devices.
-	Dynamics 365 Field Service customers can now view the service account names on the bookings screen. 
-	Updated the User Guide and Dynamics 365 Integration links in the app.
-	Update for authentication library on iOS.
-	Fix for “Just a moment” message blocking users after sign-in.
-	Fix for ArgumentNullException showing up when user don’t have any recent contacts and search query returns empty list.
-	Fix for Graphics.CopyTexture exception showing after annotating on the snapshot.
-	Fixes for application localization (e.g. “Retry sign-in” button, “Don’t show again” button and tracking error state messages).
-	Performance improvements for the application memory usage.

## iOS - 2020.5.28 + Android - 2020.05.22

Date: May 28, 2020

-	Fix for network error “HTTP 401 TeamsChatService.GetMessagesAsync”
-	Fix for application not being responsive during launch
-	Improvement for the recent contacts list 
-	Fix for not being able to find contacts in some countries, such as Egypt
-	Improvement for the voicemail card
-	Localization improvements
-	Accessibility improvements and fixes

## iOS – 2020.5.7 + Android - 2020.05.04 

Date: May 4, 2020

### Bug fixes
- Improved flighting implementation and enabling per company app customizations.
- Fix for sign in problem for users on mobile networks.
- Improved user feedback questionnaire experience.

## iOS – 2020.4.1 + Android - 2002.03.18

Date: April 1, 2020

### Bug fixes

- Fix for yellow tracking dots. Yellow tracking dots will not show up on the mobile device screen.
- Improved quality of annotations placement in the near field of 1 meter (three feet).
- Improved loading for cached recent contacts when users are in poor network condition. 
- Improved authentication handling and messaging. Better support for offline scenario and better error description.
- Fixed incorrect annotations position on tablet devices. Annotations were shifted on the sides of the screen.
- Enabled saving a snapshot if a call ends unexpectedly.
- Fixed incoming video feed position on the screen.
- Improved messaging and handling when group call is detected.
- Fixed NullReferenceException showing up during app termination and in the contacts search page.
- Fix for ArgumentOutOfRange exception showing up when typing text in the text chat.

## Locate your version number

To find which version of Remote Assist mobile you have, go to the menu and select the **Information** option. You'll see the **App Version** there. See the following screenshot for reference. 

> [!div class="mx-imgBorder"]
> ![Screenshot of Remote Assist on a mobile device, showing the information option and the app version listed.](./media/ram-version-history-locate.png)
