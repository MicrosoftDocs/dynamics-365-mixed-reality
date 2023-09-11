---
author: davepinch
description: Learn how to resolve a problem when Asset tab informs a user to contact IT admin for Dynamics 365 Remote Assist
ms.author: davepinch
ms.date: 09/12/2023
ms.topic: troubleshooting-problem-resolution
title: Asset tab indicates contact IT admin
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Asset tab indicates contact IT admin

Dynamics 365 Remote Assist says to contact my IT admin on the Assets tab

## Prerequisites

- Admin permissions in Dynamics 365 Remote Assist

## Cause 1: The app wasn't installed on the right envrionment

1. [Install the app to the right environment.](./ra-webapp-install.md#install-the-dynamics-365-remote-assist-model-driven-app)

## Cause 2: The user doesn't have the correct roles assigned

1. Verify that the user has the **Basic User** and **Remote Assist - App User** or **Remote Assist - Administrator** [security roles assigned.](./asset-capture-add-users.md#assign-dynamics-365-security-roles)

1. Close the app and the live tile, and then reopen it.