---
author: davepinch
description: Learn how to resolve a problem when the installation of the Dynamics 365 Remote Assist model-driven app fails
ms.author: davepinch
ms.date: 09/12/2023
ms.topic: troubleshooting-problem-resolution
title: The Dynamics 365 Remote Assist model-driven app failed to install
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# The Dynamics 365 Remote Assist model-driven app failed to install

Learn how to resolve a problem when the installation of the Dynamics 365 Remote Assist model-driven app fails

## Symptom

The Remote Assist model-driven app installation fails because of missing dependencies.

## Cause

If the environment isn't enabled for Dynamics 365 apps and you try to install Dynamics 365 Remote Assist, the installation fails.

## Resolution

Install the app in an environment where other Dynamics 365 apps, such as Dynamics 365 Field Service or Dynamics 365 Sales, are installed. Or  [create a new environment](#install-the-dynamics-365-remote-assist-model-driven-app) that's enabled for Dynamics 365 apps.