---
title: Content and toolkit ownership strategy
description: Learn about controlling access to guides content in the toolkit in a regulated industry.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Content and toolkit ownership strategy

When guides are authored, assets such as images, videos, and 3D objects are at the author's disposal. A toolkit that is pre-installed includes standard objects, such as pointers and arrows. All other content, such as 3D objects of machine parts and approved company logos, is provided by your organization or its suppliers.

During the implementation process, you must consider how you want to distribute ownership of, and therefore access to, content in Dynamics 365 Guides. This article uses the objects in the built-in toolkit as an example.

> [!NOTE]
> It's assumed that your organization's Microsoft Power Platform strategy is to spread data across environments and control access to guides through business units.

By default, when the Guides solution is first deployed, ownership of the toolkit elements is assigned to the user who is deploying the solution. Because several authors in your organization will probably use the toolkit elements, you can assign the ownership to a parent business unit instead. Depending on your security role settings, all users in the business unit and its associated child business units are granted access to use the toolkit elements. Because all child business units inherit the access rights of their parent unit, be careful to choose the correct ownership level to enable and restrict the access that guide authors have to content.

For example, the toolkit elements will be used by authors in a company's "A" sections (Section A1.1, Section A1.2, Section A2.1, and Section A2.2 in the following diagram). In this case, assign ownership of the elements to Department A to ensure that all the "A" sections inherit access.

:::image type="content" source="media/business-unit-structure.png" alt-text="Diagram that shows an example of business units corresponding to an organizational structure.":::

Alternatively, your organization can create a separate business unit that is named, for example, "Global Content" and assign ownership of the toolkit elements to it. Then give guide authors across the organization access to this specific business unit.

:::image type="content" source="media/3dobjects-assigned-global-content.png" alt-text="Diagram that shows an example of 3D objects assigned to a business unit in Microsoft Power Platform.":::

By carefully choosing the ownership of the toolkit, you can enable broad access to content for guide authors. However, your organization must pay regular attention to content ownership to ensure, for example, that it doesn't change if someone updates the Guides solution. Otherwise, there is a risk that authors will lose content access or be granted unauthorized access to content.

In addition, whenever Microsoft adds 3D elements to the application package, ownership must be updated after deployment (because it's automatically assigned to the deploying user).

## Next steps

- [Versioning guides strategy](strategy-for-versioning-guides.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
