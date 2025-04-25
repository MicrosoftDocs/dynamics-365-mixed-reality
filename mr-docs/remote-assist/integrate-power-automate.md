---
title: Integrate Dynamics 365 Remote Assist with Power Automate
author: prashantyvr
description: Learn how to create a Power Automate flow based on Dynamics 365 Remote Assist entities
ms.author: prashan
ms.date: 06/07/2024
ms.topic: how-to
ms.reviewer: v-wendysmith
---

# Integrate Dynamics 365 Remote Assist with Power Automate

[!INCLUDE[try-guides-ra](../includes/try-guides-ra.md)]

The asset capture feature in Remote Assist leverages Common Data Service (CDS). This feature enables you to create Power Automate flows based on the data to streamline various processes, including getting notifications, modifying other entities, and generating reports. In this article,  create a flow to get an email notification whenever a new asset attachment is created.

## Prerequisites

- Access to the environment Dynamics 365 Remote Assist is installed in.
- License and access to [Power Automate](/power-automate/).

## Create flows with Power Automate

1. Create a new flow. See [Create a cloud flow](/power-automate/get-started-logic-flow).

   1. Specify the flow's trigger as **When a record is created** and reference the **Customer Asset Attachment** record.

   1. Specify an action step as **Get record** and reference the **Customer Asset** record.

   1. Specify an action step as **Send an email notification** and reference the name of the customer asset attachment record and the name of the parent customer asset. Use both records in the subject or body of the generated email.

## Test your flow

1. Follow the steps in **[capture asset conditions](./asset-capture-photos.md)** to create a new asset capture entity record.

1. Go to the **Flows** page again to select the flow you created. On this page, you can see recent runs of the flow. Select most recent run to see its details.

1. If there are errors in the flow, you can select **Edit** to modify the flow. You can then resubmit the previous run to test your flow again, without having to create a new asset capture entity.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
