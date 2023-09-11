---
author: davepinch
description: Learn how to resolve a problem when assets don't appear in the HoloLens app for Dynamics 365 Remote Assist
ms.author: davepinch
ms.date: 09/12/2023
ms.topic: troubleshooting-problem-resolution
title: No assets appear when I select the Assets tab
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# No assets appear when I select the Assets tab

In the HoloLens app, when I select the **Assets** tab, no assets appear.

## Cause 1: Asset records weren't created in the environment

1. Ensure that the environment you're using has [asset records created](./asset-capture-create-asset.md) in it.

2. Try selecting **Retry** if you're prompted to on the **Assets** tab.

## Cause 2: Asset records were added from the model-driven app while Dynamics 365 Remote Assist was already open on HoloLens

Close the app on HoloLens and reopen it to pull the latest updates.