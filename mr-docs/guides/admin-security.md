---
author: davepinch
description: Learn how to use security groups to control which users can access which environments in Microsoft Dynamics 365 Guides.
ms.author: davepinch
ms.date: 04/24/2024
ms.topic: how-to
title: Restrict access to an environment in Dynamics 365 Guides by using security groups
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Restrict access to an environment in Dynamics 365 Guides by using security groups

If your company has multiple Microsoft Dynamics 365 Guides environments, you can use security groups to control which users can access each environment. A security group restricts access to the environment to people in the security group. If a Microsoft Dataverse environment doesn't have an associated security group, all users with a Dataverse license (Dynamics 365 Guides, Power Automate, Power Apps, and so on) are created as users and enabled in the environment. Each environment can have just one security group.

To restrict access to an environment through security groups, see [Control user access to environments with security groups](/power-platform/admin/control-user-access). 

> [!NOTE]
> Environments are sometimes referred to as "organizations" or "instances." Each of these terms refers to the same concept. 


[!INCLUDE[footer-include](../includes/footer-banner.md)]