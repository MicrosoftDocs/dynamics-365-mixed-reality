---
title: Use Microsoft Intune to protect data in Dynamics 365 Remote Assist mobile
author: amaraanigbo
description: Learn how to use Microsoft Intune to protect data in Dynamics 365 Remote Assist mobile by creating an app configuration policy for mobile devices.
ms.author: soanigbo
ms.date: 11/18/2022
ms.topic: article
ms.reviewer: mhart
---

# Use Microsoft Intune to protect data in Dynamics 365 Remote Assist mobile

Microsoft Dynamics 365 Remote Assist mobile supports Microsoft Intune's app protection policies. These policies ensure that data remains safe and contained on the device through Intune policies.  

![Graphic showing Intune controls.](./media/RAM_IntuneControls.png)

## Create an app configuration policy for mobile devices

You must be an administrator to create an app configuration policy.

1. Go to [Microsoft Endpoint Manager](https://endpoint.microsoft.com/).

1. Select **Apps**, and then select **App configuration policies**.

    ![Screenshot showing Apps and App configuration policies commands highlighted.](./media/intune-1.jpg)

1. Select **Add**, and then select **Managed apps**.

    ![Screenshot showing Add and Managed apps commands highlighted.](./media/intune-2.jpg)

1. In the **Name** field, enter the name of the policy, and then in the **Target policy to** field, choose **Selected apps**.  

    ![Screenshot showing Name and Target policy to fields highlighted.](./media/intune-3.jpg) 

1. Under **Public apps**, choose **Select public apps**.

    ![Screenshot showing Select public apps highlighted.](./media/intune-4.jpg)

1. On the right side of the screen, search for *Remote Assist*, select **Dynamics 365 Remote Assist Android** and **Dynamics 365 Remote Assist iOS**, and then choose the **Select** button.

    ![Screenshot of the right side of the screen.](./media/intune-5.jpg)

1. Select **Next** at the bottom of the screen.

1. On the **Settings** tab, do the following:

    1. Set the **Name** field to *com.microsoft.ramobile.environment.instance.url*.

    2. In the **Value** field, enter the environment url. You can find this url in the [Power Platform admin center](https://admin.powerplatform.microsoft.com). Learn more: [Create and manage environments in the Power Platform admin center](/power-platform/admin/create-environment)

    ![Screenshot of Name field and Value field filled in.](./media/intune-6.jpg)

1. Select **Next** at the bottom of the screen.

1. On the **Assignments** tab, under **Included groups**, select **Add groups**.

    ![Screenshot showing Add groups highlighted.](./media/intune-7.jpg)

1. On the right side of the screen, select the correct group for your organization, and then select **Next** at the bottom of the screen.

       ![Screenshot showing the right side of the screen.](media/intune-8.jpg)

1. On the **Review + create** tab, review the summary for the configuration policy, and then select **Create** to create the policy when you're ready.

    ![Screenshot of the Review + create tab.](./media/intune-9.jpg)

[Learn more about app configuration policies for Microsoft Intune](/mem/intune/apps/app-configuration-policies-overview)

## See also

[Dynamics 365 Remote Assist mobile overview](remote-assist-mobile-overview.md)
