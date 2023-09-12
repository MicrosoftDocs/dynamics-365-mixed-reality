---
author: davepinch
description: Learn how to resolve a problem when the assets in the HoloLens app for Dynamics 365 Remote Assist aren't what I expected or don't appear
ms.author: davepinch
ms.date: 09/12/2023
ms.topic: troubleshooting-problem-resolution
title: No assets appear or assets aren't what I expected
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# No assets appear or assets aren't what I expected

Learn how to resolve issues if no assets appear or the assets that do appear aren't what I expected to see.

## Symptoms

In the HoloLens app, when I select the **Assets** tab, the assets I see aren't what I expected to see or no assets appear.

## Cause 1: You might have access to more than one environment with Dynamics 365 Remote Assist installed

1. Select **Settings** > **Dynamics 365 environment**.

1. Select the environment.

1. Select the **Assets** tab.

1. Select **Retry** if you're prompted to on the **Assets** tab.

## Cause 2: Asset records weren't created in the environment

1. Ensure that the environment you're using has [asset records created](./asset-capture-create-asset.md) in it.

2. Select **Retry** if you're prompted to on the **Assets** tab.

## Cause 3: Asset records were added from the model-driven app while Dynamics 365 Remote Assist was already open on your HoloLens or mobile device

Close the app and reopen it to pull the latest updates.