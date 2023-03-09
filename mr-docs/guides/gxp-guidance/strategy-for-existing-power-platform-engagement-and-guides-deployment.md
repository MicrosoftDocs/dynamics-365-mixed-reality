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

# Strategy for existing Power Platform engagement and Guides deployment

Before initiating deployment of Guides, the recommendation is to investigate whether your organization already makes use of the Power Platform. If the Power Platform is well-established within your organization, you should consider whether you want to a) deploy Guides to new environments and b) let Guides co-exist in an already-existing environment with other Business Applications such as [Microsoft Dynamics 365 Field Service](https://dynamics.microsoft.com/en-ie/field-service/overview/).

To get a quick overview of any current environments within your organization and the usage hereof, you will benefit from installing the [Power Platform Center of Excellence Starter Kit](https://learn.microsoft.com/en-us/power-platform/guidance/coe/starter-kit) (CoE) within your tenant.

For regulated industries, the recommendation is to deploy Guides in new environments without the co-existence of other Business Applications, as there are certain risks related to doing so:

- **Access control mix-up** – if you deploy Guides in an existing environment with applications that has different requirements for access controls, there is a risk of mixing up the access controls and potentially allow for a wider usage of Guides than originally intended.

- **Update of applications** – if you have multiple Business Applications within the same environment, you might face difficulties whenever updates are required to the Guides application, as the other Applications within the environment, will need to pass the same tests. This can potentially slow down processes.

- **Custom code or customization** – if any of the Business Applications within the same environment use custom code and/or customization, you will need to verify that these custom features do not impact the functionality of the Guides application. Examples of such features could be changes to security roles or updates of the data model – both of which could have a direct or indirect impact on the Guides application.

- **Reference to Power Apps** - if you refer to any Power Apps (via URL) in your guides, you need to consider if these Power Apps are within the same environment as your Guides application. If not, you are advised to investigate whether the access controls applied for Guides also applies for the referenced Power Apps. To keep track of the usage and purpose of selected Power Apps, you are advised to make use of the CoE kit that contains tools to track as well as register mission-critical business apps.

If you choose to have multiple Business Applications within the same environment, you are advised to ensure that the level of criticality is the same for all applications so that the requirements for monitoring, updating, etc. are similar. However, if there is no immediate need to mix Business Applications within the same environment, the general recommendation is to separate them. This approach allows for greatest degree of control, and minimizes the risk of having multiple Business Applications, with different access controls, interfere with one another.


