---
title: Learn more about the Microsoft Dynamics 365 Remote Assist Calls Dashboard
description: Overview, enablement, and feature details for the Microsoft Dynamics 365 Remote Assist Calls Dashboard
author:  BogdanBerg
ms.author: bogdanb
ms.date: 07/08/2024
ms.topic: overview
ms.reviewer: v-wendysmith
---

# Dynamics 365 Remote Assist Calls Dashboard

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

Supervisors and operations managers need to be able to monitor key operational metrics for their organization. Such metrics are critical to get insights such as potential areas of operational efficiencies and efficacy of the various tools and processes within the technician community.

This article walks through the setup and usage of the Calls Dashboard available in the Dynamics 365 Remote Assist model-driven app. The Calls Dashboard is an opt-in feature available only to users with the security role of **Remote Assist - Administrator** or **System Administrator**.

> [!Note]
> This feature is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Remote Assist. This feature is not intended for use in making decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. End users will need to enable access from their device to phone call records and specifically consent to sharing location information before that information is shared and available through the dashboard. However, customers are also encouraged to have a mechanism in place to inform their users that analytics (such as call duration and location) relating to their communications are collected.

## Prerequisites

To have access to the Calls Dashboard, you must have:

1. Completed the steps described in the following articles:

    - [Installing the model-driven app](./ra-webapp-install.md)
    
    - [Adding users to the environment](./asset-capture-add-users.md#assign-dynamics-365-security-roles)

1. Access to the environment that Dynamics 365 Remote Assist is installed in, with the **Remote Assist - Administrator** security role assigned to you.

1. [Enable the Power BI Azure Maps visual](/azure/azure-maps/power-bi-visual-manage-access#tenant-admin-options). 

    > [!IMPORTANT]
    > Due to European privacy laws and regulations, this step only applies to customers with deployments within the US. Enabling the Power BI Azure Maps visual will not enable the map for non-US environments (for example, Europe, Canada, or Korea).  

## Enable the Calls Dashboard

1. In the Dynamics 365 Remote Assist model-driven app, under **Change area**, select **Settings**.

    ![Change area to Settings in the Remote Assist model-driven app](media/webapp-settings-selector.png).

1. Under **Analytics and Insights**, select **Settings**, and then select **Manage**.

    ![Select Calls Dashboard settings](media/CallsDashboardSettings.png).

1. Enable the dashboard.

### Notes

- The dashboard is built on Microsoft Power BI. It might take some time for the dashboard to get provisioned.

- If you see an error message that says "Map visuals aren't enabled for your org", [enable the Power BI Azure Maps visual](/azure/azure-maps/power-bi-visual-manage-access#tenant-admin-options). [Learn more about Power BI visuals admin settings](/power-bi/admin/organizational-visuals)

    > [!NOTE]
    > This error message only appears for customers with deployments outside of European (GDPR) environments. 

- The following regions don't support logging in the Calls Dashboard: GCC, GCCH, FA, ZAF, UAE, and GER. For more information, see the following links:

    - [List of regions where the Remote Assist model-driven app is deployed](ra-webapp-install.md)

    - [Complete list of Power Platform datacenter regions](/power-platform/admin/new-datacenter-regions)

- Users without a Dynamics 365 Remote Assist account/license joining a one-time call aren't shown on the Calls Dashboard.

- As a **Remote Assist - Administrator**, you can always go back and disable/re-enable the dashboard by turning it off/on from the **Settings** area. Disabling the dashboard removes the resources that it depends on.

- The dashboard uses the [phone call entity type](/dynamics365/customer-engagement/web-api/phonecall) to generate analytics. End users must [select the right Dynamics 365 environment](./asset-capture-add-users.md#selecting-the-right-environment-from-the-client-app) from their device to send the phone call record to the Microsoft Dataverse. The phone call data isn't available in the Calls Dashboard if the user didn't select the correct environment. Users can also initiate the call without selecting an environment.

    ![Selecting the correct environment for the Calls Dashboard.](media/02.07-contacts-call-prompt.png)

- End users can choose whether to give location permissions to the HoloLens app. If permission isn't granted, the location information doesn't appear in the call records for those specific users.

- If you want to enable or disable location services for all users on all devices, you can [set the **LetAppsAccessLocation** privacy policy](/windows/client-management/mdm/policy-csp-privacy#privacy-letappsaccesslocation). 

- Location information is retrieved asynchronously from the HoloLens app only after a call starts. It might be missing if the call ends abruptly or if the call is too brief (0 - 10 seconds, for example).

- If column headers aren't translated for your users when they switch languages, see [Localization of metadata](/power-automate/dataverse/known-issues).

- Data is refreshed every 24 hours. The dashboard continues to be available during the refresh. If the dashboard isn't refreshed within 24 hours, you can contact Microsoft Support. Microsoft doesn't support a custom refresh schedule.

- If an organization has no active dashboard usage for two continuous weeks, the data refresh is paused. When a user opens the dashboard, the data is refreshed in the next refresh cycle.

- Data is retained for 24 months.

- The Calls Dashboard uses storage capacity in the Microsoft Dataverse. If this increase in capacity consumption causes issues or concerns, contact Microsoft Support.

- To make sure that all calls are logged to Microsoft Dataverse, users should wait a few seconds after the call ends before closing or minimizing the Dynamics 365 Remote Assist application. 

## Understand the Dynamics 365 Remote Assist Calls Dashboard

![Screenshot of the Remote Assist Calls Dashboard](media/CallsDashboardFull.png).

### Dashboard filters

The filters available at the top of the report determine the visualizations in the dashboard. The following table describes the filters.

| Filter | Description |
| --- | --- |
| Date | Filters the dashboard to show only metrics for phone call records falling within the specified duration. |
| User name | Select specific users to view only the metrics related to them. |
| Client type | Filter the dashboard to show only metrics for phone call records coming from a specific device type. |

Additionally, when you select a slice of data from any of the visuals, the visualizations are temporarily filtered to that specific set of records. For example, if you select a specific month from the **Calls trend** visual, all visuals are filtered to that month. You can select on that data item again to remove that filter.

### Metrics available in the Calls Dashboard

Let's take a look at the information that's provided by each of the visuals in the Calls Dashboard.

| Visual | Description |
| --- | --- |
| Total calls | Total number of **unique** Dynamics 365 Remote Assist calls made. A phone call record is generated for each Dynamics 365 Remote Assist user participating in each call. No phone call record is generated for Microsoft Teams participants. Call records are disambiguated by the **RemoteAssistCallId** field in the Phone Call entity. So group calls with three or more Dynamics 365 Remote Assist users are **not** counted multiple times. |
| Total call duration | Total time spent in Dynamics 365 Remote Assist calls aggregated across all phone call records. If there are multiple Dynamics 365 Remote Assist participants in the same call, the time spent by each participant in the call is added to the total. |
| Average call duration | Average time spent in Dynamics 365 Remote Assist calls, averaged across all phone call records. |
| Unique callers | Total number of **unique** users that participated in a call from the Dynamics 365 Remote Assist app on HoloLens. This total doesn't include the number of Microsoft Teams participants. |
| Calls trend | Number of calls made over the selected duration. You can use the drill-down capabilities to see the data by year, month, week, or day. |
| Call statistics by user | The number of calls made by and time spent in Dynamics 365 Remote Assist calls per user. |
| Calls by location | Map view of the phone call records, available if the end user granted permission to share the location from their device. You can use the drill-down capabilities to see the number of calls by country/region, state, or city. |
| Call log | Details of each phone call record. Includes call start/end times, phone call record owner, call direction, time spent by the participant in the call, client device type, and location of the call participant. |

[!INCLUDE[footer-include](../includes/footer-banner.md)]
