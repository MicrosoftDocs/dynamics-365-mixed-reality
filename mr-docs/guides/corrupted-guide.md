---
author: Mamaylya
description: Learn how to avoid and fix a corrupted guide in Dynamics 365 Guides
ms.author: mamaylya
ms.date: 02/15/2023
ms.topic: how-to
title: Fix a corrupted guide in Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Fix a corrupted guide in Dynamics 365 Guides

A guide is considered corrupt when the underlying Dataverse data is not structured in a manner expected by the app. The most common cause of a corrupted guide is creating or modifying database records outside of the app. It can also happen if you give authors insufficient permission to save all data related to the guide.

## Avoid corrupting a guide

To avoid corruption:

- Delete steps and other data through the PC app only. The PC app ensures that related records are updated after a record is deleted. If you delete single records through the model-driven app or elsewhere, the guide may still contain references to the deleted record.
- Give authors at least Read, Write, Append, and Append To permissions when [sharing a guide](admin-share-guide.md). The Append To permission is necessary to link steps, tasks, and other records to the main guide record.

  :::image type="content" source="media/manage-share-access.jpg" alt-text="Manage share access screenshot":::

## Run a flow to fix a corrupted guide

You can fix a corrupted guide by running a flow in the model-driven app. This flow fixes common issues preventing the guide from being loaded. However, it can't restore deleted data and can't guarantee steps are restored exactly as ordered when the guide became corrupt. For example, if a step was deleted outside of the app, the flow removes the invalid references that are preventing the guide from loading. It is still necessary to open the guide in the PC app to re-create the missing step and manually fix step ordering.

> [!NOTE]
> If you must restore data exactly, use the [database backup and restore functions](/power-platform/admin/backup-restore-environments) in the Power Platform Admin Center.

1. [Open the model-driven app](open-model-driven-app.md).

1. Open the corrupted guide.

1. On the **Flow** menu, select **Repair corrupted guide**.

    ![Screenshot of Repair corrupted guide flow command.](media/repair-corrupted-guide-flow.jpg "Screenshot of Repair corrupted guide flow command")

1. In the **Confirmation Application of Workflow** dialog box, select **OK**.

    ![Screenshot of Workflow confirmation dialog box.](media/workflow-confirmation.jpg "Screenshot of Workflow confirmation dialog box")

1. Wait a few minutes for the flow to complete.

   [!INCLUDE [Model-driven app caution](../includes/model-driven-app-caution.md)]

## Fix steps in the PC app

The model-driven flow recreates steps in the correct places for steps that:

- Weren't saved correctly because the **Append to** permission was missing
- Were deleted in the model-driven app

Other guide steps might appear in random positions.

1. Open the guide in the PC app. Review it for incorrect steps.

   ![Screenshot of steps in the PC app after running the flow.](media/corrupted-guide-pc-app-steps.jpg "Screenshot of steps in the PC app after running the flow")

1. Add content to any recreated steps.

1. Drag steps to place them in the right order.

[!INCLUDE[footer-include](../includes/footer-banner.md)]
