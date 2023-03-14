---
title: 
description: 
ms.date: 03/13/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Strategy for versioning guides

To manage changes made to guides, use a versioning strategy. We recommend your organization distinguish between two types of versioning: major revisions and minor revisions.

**Major versions**

Whenever your organization needs a new version of a guide that exists in an execution environment, a new major version should be created. This means that a guide named "Guide 1.0" will change to "Guide 2.0". The "2.0" indicates that the updated guide has superseded a previous version. Major versioning enables tracking of changes made to the affected guides. A new major version of a guide needs to be validated, as with any other guide, before being moved to the execution stage. The version is logged in the Quality Management System (QMS) and thereby traceable.

When creating a new major version of a guide, consider what to do with the guide that the new major version supersedes:

1. Immediate retirement: retire the superseded guide to an archiving environment before authoring the new major version.

1. Supersede retirement: retire the superseded guide to an archiving environment when the new major version is approved and ready for execution.

If a procedure has changed and the current guide is no longer compliant, you might need to follow the **immediate retirement** approach as the current guide might jeopardize the safety and/or regulative procedures if instructions are launched and followed by an operator. Here, the first step is to retire the guide by moving it to archive. Next, you create, validate, and launch the new major version of the guide.

:::image type="content" source="media/immediate-retirement.png" alt-text="Example of immediate retirement":::

In another scenario, Power BI reports for usage data of the guide show that the operators pause at a specific step card. Perhaps the instructions are unclear and you want to refine them. As this update revolves around optimization and not procedural changes, there is no need to retire the current version until the new one is approved and ready for execution. In this case, the guide is not retired until it is **superseded** by the new major version.

:::image type="content" source="media/superseded-retirement.png" alt-text="Example of superseded retirement":::

**Minor versions**

Whereas major versions are mandatory, minor versions are optional. Minor versions are all version changes made before the guide reaches the execution environment. If your organization doesn't find it necessary to track the content life cycle before the execution stage, minor versions can be left out.

Only the highest minor version is transferred to the execution environment.

:::image type="content" source="media/minor-versioning.png" alt-text="Example of minor versioning":::

Versioning refers to the versioning of guides within Power Platform. This is not necessarily the same as the record versioning in QMS (the record in QMS links to the guide in Power Platform). Depending on the system and process implemented, the record version in QMS could change whenever changes are made to the metadata such as change of title or author.

We recommend that the versioning in Power Platform and the QMS is decoupled as this enables the most flexible process. Keeping the versioning synchronized can be cumbersome, as a change in versioning in QMS requires a versioning change in Power Platform. This will require a re-approval of the guide despite the change in the record in QMS not having any impact on the actual guide.

## Next steps

- [Strategy for integrations to QMS and LMS](strategy-for-integrations-to-qmslms.md)
