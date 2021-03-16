---
author: BryceHo
description: Get an overview of how to analyze guides using Microsoft Dynamics 365 Guides
ms.author: cynielse
ms.date: 03/17/2021
ms.service: crm-online
ms.topic: article
title: Overview of analyzing guides created with Dynamics 365 Guides
ms.reviewer: v-bholmes
---

# Overview of analyzing and integrating Dynamics 365 Guides operations data

When operators use the Microsoft Dynamics 365 Guides HoloLens app in Operate mode, data about guide usage is automatically stored in your private and secure Dynamics 365 environment where it can be analyzed in either of the following ways:

- Using the [Guides Analytics Power BI templates](analytics-guide.md)

- Integrated into your own custom workflows. For example, you could create a custom workflow in Microsoft Power Automate or by using third-party visualization tools or systems.

The operations data, which includes information about time spent on each step and whether an operator completed a guide, is stored in Microsoft Dataverse tables just like your Dynamics 365 Guides content. These tables make it easy to analyze guide usage across your organization, gain insights into process efficiency, or trigger worklows outside of Dynamics 365 Guides.

## How it works

|Operate a guide|Data is automatically stored|Trigger alerts or visualize data|
|----------------------------------|-----------------------------------------|-----------------------------------------|
|**Next** and **Back** button interactions are recorded to determine the time spent on each step.|Step time data is stored in your **private and secure** Dynamics 365 environment.|Use the Power Platform to analyze and act on your data.|
|![HoloLens operator at work](media/analytics-hololens-operator.PNG "HoloLens operator at work")|![Screen shot of saved step time data ](media/analytics-data-stored-automatically.PNG "Screen shot of saved step time data")|![Power Platform example](media/analytics-alerts-visualize-data.PNG "Power Platform example")|

> [!NOTE]
> Guides operations data is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making (and should not be used to make) decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. Customers are encouraged to have a mechanism in place to inform their users that analytics relating to their guides usage is collected. 

## See also

- [What data is collected and how can you use it?](analytics-data-collected.md)

- [Overview of Guides Analytics Power BI templates](analytics-guide.md)

- [Set up Guides Analytics reports](analytics-ga-setup.md)

- [Take a tour of Guides Analytics reports](analytics-ga-reports.md)

- [Share Guides Analytics reports](analytics-ga-share-reports.md)


[!INCLUDE[footer-include](../includes/footer-banner.md)]
