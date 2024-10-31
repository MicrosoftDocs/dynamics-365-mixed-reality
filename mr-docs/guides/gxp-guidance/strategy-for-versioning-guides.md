---
title: Versioning guides strategy
description: Learn about setting up a strategy for versioning guides in a regulated industry.
ms.date: 03/21/2023
ms.topic: conceptual
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Versioning guides strategy

To manage changes that are made to guides, use a versioning strategy. We recommend that your organization distinguishes two types of versions: major and minor.

## Major versions

Whenever your organization needs a new version of a guide that exists in an execution environment, create a new major version. In this case, a guide that is named "Guide 1.0" changes its name to "Guide 2.0." The "2.0" indicates that the updated guide has superseded a previous version. Major versioning enables tracking of changes that are made to the affected guides. Validate a new major version of a guide before you move it to the execution stage, just as you do for any guide. The version is logged in the quality management system (QMS) and is therefore traceable.

When you create a new major version of a guide, consider what you want to do with the guide that the new major version supersedes:

- **Immediate retirement**: Retire the superseded guide to an archiving environment before the new major version is authored.
- **Supersede retirement**: Retire the superseded guide to an archiving environment when the new major version is approved and ready for execution.

If a procedure has changed, and the current guide is no longer compliant, consider using the *immediate retirement* approach. Otherwise, safety or regulatory compliance might be at risk if an operator opens the current guide and follows the instructions in it. In this case, the first step is to retire the guide by moving it to archive. You then create, validate, and open the new major version of the guide.

:::image type="content" source="media/immediate-retirement.png" alt-text="Diagram that shows an example of immediate retirement.":::

In another scenario, Power BI reports for a guide's usage data show that operators pause at a specific step card. Because such a pause might indicate that the instructions are unclear, you decide to refine them. Because this update involves optimization, not procedural changes, there is no need to retire the current version until the new one is approved and ready for execution. Therefore, consider using the *supersede retirement* approach. In this case, the guide isn't retired until it's superseded by the new major version.

:::image type="content" source="media/superseded-retirement.png" alt-text="Diagram that shows an example of supersede retirement.":::

## Minor versions

Whereas major versions are mandatory, minor versions are optional. Minor versions are all version changes that are made before the guide reaches the execution environment. If your organization doesn't find it necessary to track the content life cycle before the execution stage, minor versions can be omitted.

Only the highest minor version is transferred to the execution environment.

:::image type="content" source="media/minor-versioning.png" alt-text="Diagram that shows an example of minor versioning.":::

In this case, *versioning* refers to the versioning of guides in Microsoft Power Platform. It isn't necessarily the same as record versioning in the QMS. (In that case, the record in the QMS is linked to the guide in Microsoft Power Platform.) Depending on the system and process that are implemented, the record version in the QMS can change whenever changes are made to the metadata, such as the title or author.

We recommend that you decouple the versioning in Microsoft Power Platform and the QMS, to make the process as flexible as possible. It can be cumbersome to keep the versioning synchronized, because a versioning change in the QMS requires a versioning change in Microsoft Power Platform. Even if the change to the record in the QMS has no impact on the actual guide, re-approval of the guide is required.

## Next steps

- [Integration with a quality management system or learning management system strategy](strategy-for-integrations-to-qmslms.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
