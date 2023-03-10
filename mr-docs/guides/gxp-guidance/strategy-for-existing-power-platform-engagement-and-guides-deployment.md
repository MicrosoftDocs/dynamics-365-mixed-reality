---
title: Strategy for existing Power Platform engagement and Guides deployment
description: Learn about using an existing Power Platform to deploy Guides
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
---

# Strategy for existing Power Platform engagement and Guides deployment

Before initiating deployment of Guides, the recommendation is to investigate whether your organization already makes use of the Power Platform. If the Power Platform is well-established within your organization, you should consider whether you want to deploy Guides to new environments or let Guides co-exist in an already-existing environment with other business applications such as [Microsoft Dynamics 365 Field Service](https://dynamics.microsoft.com/field-service/overview/).

To get a quick overview of any current environments within your organization and the usage, install the [Power Platform Center of Excellence Starter Kit](/power-platform/guidance/coe/starter-kit) (CoE) within your tenant.

For regulated industries, we recommend deploying Guides in new environments without the co-existence of other business applications, due to certain risks:

- **Access control mix-up** – if you deploy Guides in an existing environment with applications that have different requirements for access control, there is a risk of mixing up the access controls and potentially allowing a wider usage of Guides than originally intended.

- **Update of applications** – if you have multiple business applications within the same environment, you might face difficulties whenever updates are required to the Guides application, as the other applications within the environment must pass the same tests. This can potentially slow down processes.

- **Custom code or customization** – if any of the business applications within the same environment use custom code and/or customization, verify that these custom features do not impact the functionality of the Guides application. For example, custom changes to security roles or updates of the data model can have a direct or indirect impact on the Guides application.

- **Reference to Power Apps** - if you refer to any Power Apps via URL in your guides, consider if these Power Apps are within the same environment as your Guides application. If not, we recommend you investigate whether the access controls applied for Guides also applies for the referenced Power Apps. To keep track of the usage and purpose of selected Power Apps, we recommend using the CoE kit tools to track and register mission-critical business apps.

If you choose to have multiple business applications within the same environment, we recommend you ensure that the level of criticality is the same for all applications so that the requirements for monitoring, updating, and others are similar. However, if there is no immediate need to mix business applications within the same environment, the general recommendation is to separate them. This approach allows for the greatest degree of control and minimizes the risk of having multiple business applications with different access controls interfere with one another.
