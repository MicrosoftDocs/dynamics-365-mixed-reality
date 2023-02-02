---
author: Mamaylya
description: Learn how to use security groups to control which users can access which environments in Microsoft Dynamics 365 Guides.
ms.author: mamaylya
ms.date: 12/14/2021
ms.topic: article
title: Restrict access to an environment in Dynamics 365 Guides by using security groups
ms.reviewer: v-wendysmith
---

# Restrict access to an environment in Dynamics 365 Guides by using security groups

If your company has multiple Microsoft Dynamics 365 Guides environments, you can use security groups to control which users can access each environment. A security group restricts access to the environment to people in the security group. If a Microsoft Dataverse environment does not have an associated security group, all users with a Dataverse license (Dynamics 365 Guides, Power Automate, Power Apps, and so on) will be created as users and enabled in the environment. 

Each environment can have just one security group. For example, you could create three security groups to control access to the following environments.

| Environment                    | Security group  | Purpose |
|--------------------------------|-----------------|---------|
| Coho Manufacturing Sales       | Sales\_SG       | Provide access to the organization that creates sales opportunities, handles quotations, and closes deals. |
| Coho Manufacturing Maintenance | Maintenance\_SG | Provide access to the organization that does service and machinery maintenance. |
| Coho Manufacturing Dev         | Developer\_SG   | Provide access to the sandbox environment that is used for development and testing. |

[Learn more about controlling user access to environments with security groups](/power-platform/admin/control-user-access). 

> [!NOTE]
> Environments are sometimes referred to as "organizations" or "instances." Each of these terms refers to the same concept. 

## See also

- [Control user access to environments: security groups and licenses](/power-platform/admin/control-user-access)

- [Add several users at the same time](/office365/enterprise/add-several-users-at-the-same-time)

[!INCLUDE[footer-include](../includes/footer-banner.md)]