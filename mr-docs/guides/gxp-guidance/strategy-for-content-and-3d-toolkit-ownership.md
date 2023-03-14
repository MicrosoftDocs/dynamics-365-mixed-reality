---
title: Strategy for content and 3D Toolkit ownership
description: Learn about controlling access to guides content in the 3D Toolkit in a regulated industry
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Strategy for content and 3D Toolkit ownership

When authoring guides, assets such as images, videos, and 3D objects are at the author's disposal. A 3D toolkit with standard objects such as pointers and arrows are pre-installed, while all additional content such as a 3D model of a machine part or approved company logos, are provided by your organization or its suppliers.

In the implementation process, consider how to distribute ownership and hereby access to content within Guides. Let's take the objects in the built-in 3D toolkit as an example:

> [!NOTE]
> It is assumed that your organization's Power Platform strategy is to spread data across environments and control access to guides via business units.

When the Guides solution is initially deployed, by default, the ownership of the 3D toolkit elements is assigned to the user deploying the solution. Since the 3D toolkit elements are likely to be used by several authors in your organization, you can assign the ownership to a parent business unit instead. If allowed by your security role settings, all users in the business unit and its associated child business units are given access to utilize the toolkit elements. Because all child business units inherit the access rights of its parent unit, be careful to choose the right ownership level to enable as well as restrict guides authors' content access.  
  
For instance, if the toolkit elements are to be used by authors in a company's A-sections, for example, ownership of the 3D toolkit elements must be assigned to "Department A" for all the A-sections ("Section A1.1", "Section A1.2", "Section A2.1", and "Section 21.2") to inherit access.

:::image type="content" source="media/business-unit-structure.png" alt-text="Example of business units corresponding to an organizational structure ":::

Alternatively, your organization can create a separate business unit named, for example, "Global Content", and assign 3D toolkit element ownership to this unit. Subsequently, you'll give guides authors across the organization access to this separate unit specifically.

:::image type="content" source="media/3dobjects-assigned-global-content.png" alt-text="Example of 3D objects assigned to a business unit in Power Platform":::

Carefully choosing the ownership of the 3D toolkit can enable broad access to content for guides authors. However, it is necessary to regularly pay attention to content ownership. For instance, when someone updates the Guides solution, your organization needs to check that content ownership does not change. Otherwise, authors risk losing content access, or authors are granted unauthorized access to content.

Also, whenever Microsoft adds 3D elements to the application package, ownership will need to be updated post deployment due to the automatic ownership assignment to the deploying user.

## Next steps

- [Strategy for versioning guides](strategy-for-versioning-guides.md)
