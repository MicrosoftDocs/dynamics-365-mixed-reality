---
title: Learn more about the Remote Assist Calls Dashboard
author: dhgoelmsft
description: Overview, enablement and feature details of Remote Assist Calls Dashboard
ms.author: dhgoel
ms.date: 09/28/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---

# Dynamics 365 Remote Assist Calls Dashboard

Supervisors and operations managers need to be able to monitor key operational metrics for their organization. Such metrics are critical to get insights such as potential areas of operational efficiencies and efficacy of the various tools and processes within the technician community.

This article walks through the setup and usage of the calls dashboard feature available in the Dynamics 365 model-driven app. Calls dashboard is an opt-in feature available only to users with the security role of **Remote Assist - Administrator** or **System Administrator**.

:::image type="content" source="media/CallsDashboardFull.png" alt-text="Screenshot of the Remote Assist Calls Dashboard.":::

> [!Note]
> This feature is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Remote Assist. This feature is not intended for use in making—and should not be used to make—decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. End users will need to consent to sharing location information from their devices before that information is shared and available through the dashboard, but customers are also encouraged to have a mechanism in place to inform their users that their communications be monitored for the purpose of collecting analytics.

## Prerequisites

To have access to the calls dashboard, you must have:

1. Completed the steps described in the following articles:

    1. [Installing the model-driven app](./ra-webapp-install.md)
    2. [Adding users to the environment](./asset-capture-add-users.md#assign-dynamics-365-security-roles)

1. Access to the environment Dynamics 365 Remote Assist is installed in, with the **Remote Assist - Administrator** security role assigned to you.

## Enabling the calls dashboard

1. From the Remote Assist model-driven app, change the area by clicking on the menu in the bottom left of the screen and select **Settings**.
:::image type="content" source="media/webapp-settings-selector.png" alt-text="Change area to Settings in the Remote Assist model-driven app":::

2. Select **Settings** under **Analytics and Insights** and click on **Manage**.
:::image type="content" source="media/CallsDashboardSettings.png" alt-text="Select Calls Dashboard settings":::

3. Click on the toggle to enable the dashboard.
:::image type="content" source="media/CallsDashboardEnable.png" alt-text="Toggle on Calls Dashboard":::

### Notes

1. It may take some time for the dashboard to get provisioned.

1. As **Remote Assist - Administrator**, you can always go back and disable the dashboard by toggling it off from within the **Settings** area as described above.

1. The dashboard leverages the phonecall entity type to generate analytics. End users must select the right Dynamics environment from their device to send the phonecall record to the Common Data Service. Only after they have selected the correct environment, and for those users only, is the phonecall data available in the calls dashboard. 

1. End users may or may not give location permissions to the Hololens or Mobile app. If permission is not granted, for call records from those specific users, location information will be missing.