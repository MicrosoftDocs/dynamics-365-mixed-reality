---
author: Mamaylya
description: Learn what kind of call data is stored by Dynamics 365 Guides
ms.author: davepinch
ms.date: 06/23/2023
ms.topic: overview
title: Call data stored by Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Call data stored by Dynamics 365 Guides

When Microsoft Dynamics 365 Guides users make or receive calls in the HoloLens app, call information is stored in Microsoft Dataverse.

Location data is only stored in Microsoft Dataverse if the user consents to store that data. Users are prompted to provide [permission](hololens-permissions.md) to store location data when they start the HoloLens app for the first time. If a user chooses not to store location data, other calling information is stored, but location fields in the app will be empty. [Learn more about HoloLens app permissions](hololens-permissions.md).

## What data is stored and when

> [!NOTE]
> Dynamics 365 Guides stores call data in a persistent queue on the client. If the call data isn't uploaded the first time, Dynamics 365 Guides attempts to  upload the data three more times at different time intervals. This increases the reliability of data uploading.

Some of the fields listed below are not visible in the default form for the PhoneCall table, but the data is still available and can be accessed in any of the following ways:

- Using [Advanced Find](/power-apps/user/advanced-find)
- Browsing the data model in https://make.powerapps.com
- Doing your own customizations

### Data updated at the start of a call

The following data is updated at the start of the call:

- CallId
- CallStart
- CallEnd (set to the same value as CallStart at the beginning of the call, and then updated at the end of the call)
- ClientType (possible values: **HoloLens**, **HoloLens 2**, **Android**, **iOS**)
- Subject (set to **Dynamics 365 Guides**)
- IsOutgoing

### Data updated soon after a call starts

The following data is updated soon (within 2-5 seconds) after the start of the call, but only if the user provided permission to store location data:

- City (the city where the call was placed)
- StateOrProvince
- Country
- Latitude
- Longitude

### Data updated at the end of a call

The following data is updated at the end of the call, but only if the Dynamics 365 Guides app is in foreground:

- CallDurationMinutes (duration of the call in minutes)
- CallDurationSeconds
- CallEnd
- StateCode (set to **Completed** at the end of the call)
- StatusCode (set to **Made** or **Received**)

### Fields that don't have values in the Phone Calls form

The following fields in the **Phone Calls** form are empty (don't have displayed values):

- Call From
- Call To
- Phone Number
- Description
- Regarding

Dynamics 365 Guides doesn't store values in these fields, but they're included because the form is shared with other Microsoft products such as Dynamics 365 Field Service.

## Next steps

- [View and access Guides call data](call-logging.md)

[!INCLUDE[footer-include](../includes/footer-banner.md)]
