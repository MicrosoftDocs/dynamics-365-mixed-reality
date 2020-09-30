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

> [!Note]
> This feature is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Remote Assist. This feature is not intended for use in making—and should not be used to make—decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. End users will need to consent to sharing location information from their devices before that information is shared and available through the dashboard, but customers are also encouraged to have a mechanism in place to inform their users that their communications be monitored for the purpose of collecting analytics.

## Prerequisites

To have access to the calls dashboard, you must have:

1. Completed the steps described in the following articles:

    1. [Installing the model-driven app](./ra-webapp-install.md)
    2. [Adding users to the environment](./asset-capture-add-users.md#assign-dynamics-365-security-roles)

1. Access to the environment Dynamics 365 Remote Assist is installed in, with the **Remote Assist - Administrator** security role assigned to you.

## Enabling the calls dashboard

1. From the Remote Assist model-driven app, change the area by clicking on the menu in the bottom left of the screen and select **Settings**.\
:::image type="content" source="media/webapp-settings-selector.png" alt-text="Change area to Settings in the Remote Assist model-driven app":::

2. Select **Settings** under **Analytics and Insights** and click on **Manage**.
:::image type="content" source="media/CallsDashboardSettings.png" alt-text="Select Calls Dashboard settings":::

3. Click on the toggle to enable the dashboard.
:::image type="content" source="media/CallsDashboardEnable.png" alt-text="Toggle on Calls Dashboard":::

### Notes

1. The dashboard is built on Microsoft Power BI. It may take some time for the dashboard to get provisioned.

1. As **Remote Assist - Administrator**, you can always go back and disable the dashboard by toggling it off from within the **Settings** area as described above.

1. The dashboard leverages the [phonecall entity type](https://docs.microsoft.com/dynamics365/customer-engagement/web-api/phonecall) to generate analytics. End users must [select the right Dynamics environment](./asset-capture-add-users.md#selecting-the-right-environment-from-the-client-app) from their device to send the phonecall record to the Common Data Service. Only after they have selected the correct environment, and for those users only, is the phonecall data available in the calls dashboard.

1. End users may or may not give location permissions to the Hololens or Mobile app. If permission is not granted, for call records from those specific users, location information will be missing.

## Understanding the Dynamics 365 Remote Assist calls dashboard

:::image type="content" source="media/CallsDashboardFull.png" alt-text="Screenshot of the Remote Assist Calls Dashboard.":::

### Dashboard filters

All visuals described are governed by the filters available at the top of the report. Let's understand what these filters do.

| Filter | Description |
| --- | --- |
| Date | Filters the dashboard to only show metrics for phonecall records falling within the specified duration. |
| User name | Select specific users to view only metrics related to them. |
| Client type | Filter the dashboard to only show metrics for phonecall records coming from a specific device type. |

Additionally, when you select a slice of data from any of the visuals described below, it will temporarily filter all visuals to that specific set of records. For e.g., if you click on a specific month from the **calls trend** visual, all visuals will be filtered to that month. You can click on that data item again to remove that filter.

### Metrics available in the calls dashboard

Let's take a look at what information is provided by each of the visuals in the calls dashboard.

| Visual | Description |
| --- | --- |
| Total calls | Total number of **unique** Dynamics 365 Remote Assist calls made. There is a phonecall record generated for each Dynamics 365 Remote Assist user participating in each call. There is no phonecall record generated for Microsoft Teams participants. Call records are disambiguated by the **RemoteAssistCallId** field in the phonecall entity. Thus group calls, with three or more Dynamics 365 Remote Assist users are **not** counted multiple times. |
| Total call duration | Total time spent in Dynamics 365 Remote Assist calls aggregated across all phonecall records. If there are multiple Dynamics 365 Remote Assist participants in the same call, the time spent by each participant in the call will be added to the total. |
| Average call duration | Average time spent in Dynamics 365 Remote Assist calls, averaged across all phonecall records. |
| Unique callers | Total number of **unique** users that participated in a call from the Dynamics 365 Remote Assist app on HoloLens or Mobile. This does not include the number of Microsoft Teams participants. |
| Calls trend | Number of calls made over the selected duration. You can use the drill down capabilities of the visual to see the data by year, month, week or day. |
| Call statistics by user | The number of calls made by and time spent in Dynamics 365 Remote Assist calls per user. |
| Calls by location | Map view of the phonecall records, available if the end user has granted permission to share location from their device. You can use the drill down capabilities of the visual to see number of calls by country, state or city. |
| Call log | Details of each phonecall record, including call start and end times, owner of the phonecall record, direction of the call, time spent by the specific participant in the call, client device type, and location of the call participant if shared. |

## Additional notes

* **SLA**: Data is refreshed every 24 hours. Dashboard will continue to be available during the refresh. If the dashboard is not refreshed within 24 hours, you can contact Microsoft Support. Please note that currently, we do not support a custom refresh schedule.

* **Data Refresh for Inactive environments**: If an organization has no active usage of the dashboard for two continuous weeks, the data refresh will be paused. When a user opens the dashboard, the data will get refreshed in the next refresh cycle.

* Data is retained for 24 months.

* The calls dashboard feature uses storage capacity in the Common Data Service. If this increase in capacity consumption causes issues or concerns, contact Microsoft Support.
