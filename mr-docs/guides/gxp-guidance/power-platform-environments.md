---
title: Microsoft Power Platform environments
description: Learn how to set up and maintain Microsoft Power Platform environments for use with Dynamics 365 Guides.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Microsoft Power Platform environments

Learn how to set up and maintain [environments](/power-platform/admin/environments-overview) in Microsoft Power Platform.

## Microsoft Power Platform environment setup

Use [Power Platform admin center](https://aka.ms/ppac) to complete administrative tasks for environments. Your organization will perform the following tasks, among others:

- [Create environments](/power-platform/admin/create-environment).
- [Control environments](/power-platform/admin/control-environment-creation).
- [Add databases](/power-platform/admin/create-database).
- [Configure approved environment capacity](/power-platform/guidance/coe/capacity-alerting).
- [Enable Dataverse audit logging](/power-platform/guidance/adoption/cds-usage#dataverse-audit-logging).
- [Delete](/power-platform/admin/delete-environment), [recover](/power-platform/admin/recover-environment), [reset](/power-platform/admin/reset-environment), [copy](/power-platform/admin/copy-environment) and [back up](/power-platform/admin/backup-restore-environments) environments.

We recommend that you set up a governance structure for handling and managing the administrative tasks. This governance is relevant from a consumption and compliance perspective. If multiple employees in your organization create environments for purposes such as training and testing, Microsoft Power Platform automatically allocates storage to those environments. If environments are created occasionally and then forgotten, the unused environments will continuously drive consumption and cost for your organization. More importantly, unmanaged environments aren't compliant in terms of a transparent audit trail that can be followed.

If your organization hasn't yet adopted Microsoft Power Platform, or if it's low in maturity, consider exploring the [Microsoft Power Platform Center of Excellence (CoE) Starter Kit](/power-platform/guidance/coe/starter-kit).

## Microsoft Power Platform environment maintenance

To maintain your Microsoft Power Platform environments, we recommend that your organization:

- Continuously [monitors environment adoption, usage, and health](/power-platform/guidance/adoption/cds-usage) through metrics such as the number of active users and API calls (pass rate and top failures). A [weekly email digest](/power-platform/admin/managed-environment-usage-insights) that includes analytics can be provided.
- Creates [data loss prevention policies](/power-platform/admin/wp-data-loss-prevention) at the environment or tenant level to help prevent users from unintentionally exposing, misusing, or losing organizational data.
- Reacts to [capacity alerts](/power-platform/guidance/coe/capacity-alerting#receive-capacity-alerts). If approved environment capacity is configured, Microsoft Power Platform admins are notified when environments are at 80-percent approved capacity or more. If allocated capacity at the tenant level is exceeded, [some operations](/power-platform/admin/capacity-storage#changes-for-exceeding-storage-capacity-entitlements) become prohibited. This scenario can arise if, for example, you're working with large 3D objects in Dynamics 365 Guides.

### Software compatibility

Check [Guides software compatibility](../admin-apps-solution-compatibility.md). The software versions of Guides on PCs, on HoloLens devices, and in Microsoft Power Platform environments must be compatible with each other. Otherwise, users on the PCs and the HoloLens devices receive an error message that prompts them to contact their admin because of non-updated software.

It's critical that you have governance for software compatibility and a well-established process to ensure that all risk is assessed, tested, and in sync with Microsoft's Guides release cycle.

### Feature roadmap

To stay on top of upcoming Microsoft Power Platform features and potential changes to your governance structure, familiarize yourself with the current [Microsoft Power Platform release plan](/dynamics365/release-plans/).

## Next steps

- [Anchor guide content through QR codes and embed deep links](anchor-guides-content-through-qr-codes-and-embed-deep-links.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
