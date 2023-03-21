---
title: Power Platform environments
description: Learn how to setup and maintain Power Platform environments to use with Dynamics 365 Guides
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Power Platform environments

Learn how to setup and maintain [environments](/power-platform/admin/environments-overview) in Power Platform.

## Power Platform environment setup

To administer environments, the [Power Platform admin center](https://aka.ms/ppac) is used to complete administrative tasks. Your organization will perform the following tasks, among other things:

- [Create](/power-platform/admin/create-environment) environments
- [Control](/power-platform/admin/control-environment-creation) environments
- [Add databases](/power-platform/admin/create-database)
- [Configure approved environment capacity](/power-platform/guidance/coe/capacity-alerting)
- [Enable Dataverse audit logging](/power-platform/guidance/adoption/cds-usage#dataverse-audit-logging)
- [Delete](/power-platform/admin/delete-environment), [recover](/power-platform/admin/recover-environment), [reset](/power-platform/admin/reset-environment), [copy](/power-platform/admin/copy-environment) and [backup](/power-platform/admin/backup-restore-environments) environments

We recommend setting up a governance structure for handling and managing the administrative actions. This is relevant from a consumption as well as compliance perspective. If multiple employees within your organization create environments, for instance for training and testing, storage is automatically allocated to these environments by Power Platform. If environments are created every now and then and forgotten, unused environments will continuously drive consumption and cost for your organization. More importantly, unmanaged environments aren't compliant in terms of creating a transparent, followable audit trail.

If your organization hasn't adopted Power Platform yet or is low in maturity, consider exploring the [Power Platform Center of Excellence (CoE) Starter kit](/power-platform/guidance/coe/starter-kit).

## Power Platform environment maintenance

To maintain your Power Platform environments, we recommend to:

- [Monitor environment adoption, usage, and health](/power-platform/guidance/adoption/cds-usage) continuously through metrics such as number of active users and API calls (pass rate and top failures). A [weekly email digest](/power-platform/admin/managed-environment-usage-insights) with analytics can be provided.
- Create [data loss prevention policies](/power-platform/admin/wp-data-loss-prevention) at environment or tenant level to help prevent users from unintentionally exposing organizational data, misuse it, or lose it.
- React on [capacity alerts](/power-platform/guidance/coe/capacity-alerting#receive-capacity-alerts). If approved environment capacity is configured, Power Platform admins are notified when environments are at 80% approved capacity or above. If allocated capacity at tenant level is exceeded, [certain operations](/power-platform/admin/capacity-storage#changes-for-exceeding-storage-capacity-entitlements) become prohibited. This scenario could, for example, play out if you are working with large 3D models in Guides.

**Software compatibility**

Check [Guides software compatibility](../admin-apps-solution-compatibility.md): The software versions of Guides on PC, HoloLens, and Power Platform environments must be compatible with each other. If not, the end-user on the PC and the HoloLens receive an error message asking them to contact their admin because of non-updated software.

It is critical to have software compatibility under governance and have a well-established process to ensure all is risk assessed, tested and in synch to the release cycle of Guides by Microsoft.

**Feature roadmap**

To stay on top of coming Power Platform features and potential changes to your governance structure, familiarize yourself with the current [Power Platform release plan](/dynamics365/release-plans/).

## Next steps

- [Governance - Anchor guides content](anchor-guides-content-through-qr-codes-and-embed-deep-links.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
