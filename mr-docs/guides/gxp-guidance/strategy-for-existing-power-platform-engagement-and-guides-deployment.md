---
title: Existing Microsoft Power Platform engagement and Guides deployment strategy
description: Learn about using an existing Microsoft Power Platform engagement to deploy Dynamics 365 Guides in a regulated industry.
ms.date: 03/20/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Existing Microsoft Power Platform engagement and Guides deployment strategy

Before you initiate deployment of Dynamics 365 Guides, we recommend that you investigate whether your organization already uses Microsoft Power Platform. If Microsoft Power Platform is well-established in your organization, consider whether you want to deploy Guides to new environments or let it co-exist with other business applications, such as [Dynamics 365 Field Service](https://dynamics.microsoft.com/field-service/overview/), in an existing environment.

To get a quick overview of any current environments in your organization, and their usage, install the [Microsoft Power Platform Center of Excellence (CoE) Starter Kit](/power-platform/guidance/coe/starter-kit) in your tenant.

For regulated industries, we recommend that you deploy Guides in new environments where it won't co-exist with other business applications. Otherwise, there are some risks:

- **Access control mix-up**: If you deploy Guides in an existing environment with applications that have different requirements for access control, there is a risk that the access control will become mixed up, allowing Guides to be used more widely than was originally intended.
- **Update of applications**: If you have multiple business applications in the same environment, you might encounter issues whenever updates to the Guides application are required. Because the other applications in the environment must pass the same tests, there is a risk that processes will be slowed down.
- **Custom code or customization**: If any of the business applications in the same environment use custom code or customization, verify that none of these custom features affect the functionality of the Guides application. For example, custom changes to security roles or updates of the data model can have a direct or indirect impact on the Guides application.
- **Reference to Power Apps**: If you refer to any apps that were developed in Power Apps via URLs in your guides, determine whether those apps are in the same environment as the Guides application. If they aren't, we recommend that you investigate whether the access controls that are applied to Guides also apply to the referenced apps. To keep track of the usage and purpose of selected apps, we recommend that you use the tools in the CoE kit to track and register mission-critical business apps.

If you choose to have multiple business applications in the same environment, we recommend that you ensure that all of them have the same level of criticality. In this way, they will have similar requirements for monitoring, updates, and so on. However, if there is no immediate need to mix business applications in the same environment, the general recommendation is that you separate them. This approach allows for the greatest degree of control and minimizes the risk that business applications that different have access control will interfere with each another.

## Next steps

- [Security and separation of environment access strategy](strategy-for-security-and-separation-of-environment-access.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
