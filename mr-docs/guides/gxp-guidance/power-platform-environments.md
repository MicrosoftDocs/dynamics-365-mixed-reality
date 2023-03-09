---
title: 
description: 
ms.date: 03/09/2023
ms.topic: 
ms.service: 
author: 
ms.author: 
manager: 
---

# Power Platform Environments

This section concerns the setup and maintenance of [environments](https://learn.microsoft.com/en-us/power-platform/admin/environments-overview) in the Power Platform.

## Setup Power Platform environments

To administer environments, the [<u>Power Platform admin center</u>](https://aka.ms/ppac) is used to complete administrative tasks. Your organization will perform the following tasks, among other things:

-   [create](https://learn.microsoft.com/en-us/power-platform/admin/create-environment) environments

-   [control](https://learn.microsoft.com/en-us/power-platform/admin/control-environment-creation) environments

-   [add databases](https://learn.microsoft.com/en-us/power-platform/admin/create-database)

-   [configure approved environment capacity](https://learn.microsoft.com/en-us/power-platform/guidance/coe/capacity-alerting)

-   [enable Dataverse audit logging](https://learn.microsoft.com/en-us/power-platform/guidance/adoption/cds-usage#dataverse-audit-logging)

-   [delete](https://learn.microsoft.com/en-us/power-platform/admin/delete-environment), [recover](https://learn.microsoft.com/en-us/power-platform/admin/recover-environment), [reset](https://learn.microsoft.com/en-us/power-platform/admin/reset-environment), [copy](https://learn.microsoft.com/en-us/power-platform/admin/copy-environment) and [backup](https://learn.microsoft.com/en-us/power-platform/admin/backup-restore-environments) environments.

It is recommended to set up a governance structure for handling and managing the administrative actions. This is relevant from a consumption as well as compliance perspective. If multiple employees within your organization create environments, for instance for training and testing, storage will automatically be allocated to these environments by the Power Platform. If environments are created every now and then and forgotten, unused environments will continuously drive consumption and cost for your organization. Even more importantly, unmanaged environments will not be compliant in terms of creating a transparent, followable audit trail.

If your organization has not adopted Power Platform yet or is low in maturity, consider exploring the [Power Platform Center of Excellence (CoE) Starter kit](https://learn.microsoft.com/en-us/power-platform/guidance/coe/starter-kit).

## Maintain Power Platform environments

To maintain your Power Platform environments, it is recommended to:

-   continuously [monitor environment adoption, usage, and health](https://learn.microsoft.com/en-us/power-platform/guidance/adoption/cds-usage) through metrics such as number of active users and API calls (pass rate, top failures, etc.). A [weekly email digest](https://learn.microsoft.com/en-us/power-platform/admin/managed-environment-usage-insights) with analytics can be provided.

-   create [data loss prevention policies](https://learn.microsoft.com/en-us/power-platform/admin/wp-data-loss-prevention) at environment or tenant level to help prevent users from unintentionally exposing organizational data, misuse it, or lose it.

-   react on [capacity alerts](https://learn.microsoft.com/en-us/power-platform/guidance/coe/capacity-alerting#receive-capacity-alerts). If approved environment capacity is configured, Power Platform admins will be notified when environments are at 80% approved capacity or above. If allocated capacity at tenant level is exceeded, [certain operations](https://learn.microsoft.com/en-us/power-platform/admin/capacity-storage#changes-for-exceeding-storage-capacity-entitlements) become prohibited. This scenario could, for example, play out if you are working with large 3D models in Guides.

**Software compatibility  
**Check [Guides software compatibility](https://learn.microsoft.com/en-us/dynamics365/mixed-reality/guides/admin-apps-solution-compatibility): The software versions of Guides on PC, HoloLens, and Power Platform environments must be compatible with each other. If not, the end-user on PC and HoloLens will face an error message asking you to contact your admin because of non-updated software. 

This is a critical area to have under governance and have a well-established process for. This is for ensure all is in risk assessed, tested and in synch to the release cycle by Microsoft of Guides

**Feature roadmap**

To stay on top of coming Power Platform features and potential changes to your governance structure, familiarize yourself with the current [Power Platform release plan](https://learn.microsoft.com/en-us/dynamics365/release-plans/).

 

 

## Governance


