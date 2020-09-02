---
author: Makamat
description: Learn how to opt out of storing Microsoft Dynamics 365 Guides usage data in Common Data Service, for privacy reasons.
ms.author: makamat
ms.date: 09/02/2020
ms.service: crm-online
ms.topic: article
title: Opt out of storing Dynamics 365 Guides usage data in Common Data Service
ms.reviewer: v-brycho
---

# Opt out of storing Dynamics 365 Guides usage data in Common Data Service

Dynamics 365 Guides apps enable teams to capture usage statistics and detailed time-tracking information. This data is used to 
provide metrics for operator performance and help you identify opportunities for process optimization. Administrators can turn off 
data collection for specific users if they like. 

To do this:

1.	Go to powerapps.microsoft.com and sign in with your admin account.

2.	In the tenant/instance drop-down, select the instance that has Dynamics 365 Guides installed.

3.	Select the Guides app in the list. This opens a new tab for the Guides model-driven app.

    > [!NOTE]
    > The Guides model-driven app is not intended to be used as a replacement for authoring with the PC and HoloLens apps. If you create, update, or delete records using the model-driven app, you might make Guides non-functional, or prevent users from using the PC or HoloLens apps in the intended way. Modification by way of the model-driven app is not fully supported at this time and should be reserved for experienced Dynamics 365 developers familiar with the Common Data Service.

4.	In the left navigation, go to **User Settings.**

    ![User Settings](media/data-opt-out-user-setting.PNG "User Settings")
 
5.	Select **New**.

    ![Select New](media/data-opt-out-new.PNG "Select New")
 
6.	Fill out the form as follows:

    - **Name:** Opt out for *add user name here*.

    - **Record Guide Usage:** Yes.

    - **Belongs To:** User's name. 

7.	Select **Save**.

    ![Filled-out form](media/data-opt-out-filled-out-form.PNG "Filled-out-form")
 
## See also

[Analyze guides usage](analytics-guide.md)
