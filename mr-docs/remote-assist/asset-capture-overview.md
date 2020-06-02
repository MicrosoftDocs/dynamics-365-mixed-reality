---
title: Asset Capture Overview 
author: bencorn
description: Overview of the Asset Capture Public Preview 
ms.author: becorn
ms.date: 5/30/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Asset Capture Public Preview Overview

## Overview
The Asset Capture public preview introduces non-calling scenarios in Remote Assist by enabling technicians to capture data about the assets they operate, inspect, and maintain. The data is captured in a consistent and structured way for easy validation, report generation, and auditing.

Compared to the snapshot tool currently available in Remote Assist for capturing data, asset capture has several additional benefits:

- **Available independent of calls**: technicians can use Remote Assist to capture processes such as inspections, audits, repair procedures, and factory acceptance tests **independent of a call**. This is great for scenarios where they are working by themselves or a video call is not possible. Simply put, asset capture, spatial markup tools, and reference documents are now always available from the second you start Remote Assist.
- **More flexible and robust**: Asset Capture is built on Common Data Service and the Common Data Model. Data generated in Remote Assist can be used in automated processes with Power Automate Flows or in your existing Dynamics 365 apps and Power Apps. Because Remote Assist uses the same Customer Asset entity used in Field Service and Connected Customer Service, Remote Assist seamlessly extends those applications, enabling technicians to capture spatial data to the asset in Remote Assist.
- **Easier to manage**: Data captured with Asset Capture is automatically related back to a digital record of the equipment (assets) you maintain or operate. Overtime, these records become a historical record and audit trail of rich spatial data captured from Remote Assist. And compared to OneDrive where the user must share the folder with specific individuals to view, asset data is saved to Common Data Service so anyone in the organization with access to Common Data Service (CDS) can view that data.

Asset Capture is easy to start using and involves the following steps:

1. Administrator installs the Dynamics 365 Remote Assist app on a Dynamics 365 environment
2. Administrator adds Remote Assist users to the environment
3. Administrator manually creates digital asset records or imports existing data to Remote Assist
4. Technician enables the Asset Capture preview on their HoloLens
5. Technician completes their work, such as an inspection, and captures the inspection data to the asset record through Remote Assist.
6. View the captured data.

> [!NOTE]
> Asset Capture is in public preview and currently only available on HoloLens 2. The feature is disabled by default when you download the update to ensure your current users are not impacted by the workflow changes in this update. The following tutorials will guide you through how to get started with Asset Capture, including enabling the features in the HoloLens 2.

## Next steps

Get started with the Asset Capture public preview by starting with this tutorial:

> [!div class="nextstepaction"]
> [Setup an environment](./asset-capture-setup-environment.md)

## Entity Reference

Asset Capture uses several entities stored in Common Data Model:

1. Customer Asset: the individual asset.
2. Customer Asset Category: a way to describe a group of similar assets.
3. Customer Asset Attachment: a media item captured in HoloLens of a single asset.
4. Account: the customer account where the asset currently exists.
5. Product: the make/model of the asset.

## Additional notes

- Support for HoloLens 1 and Mobile isn't part of the June public preview and is **planned**.
- Support for video capture isn't available in the June release and is **planned**
- During sign-in, Remote Assist will try to automatically select the first environment the user has access to with the Remote Assist app installed. If the user has access to more than one environment with the Remote Assist app installed, you can select the desired environment by selecting **Settings** > **Links** > **Switch Dynamics Instance**.

### Known issues

- Users with access to a large number of environments will experience long delays the first time they sign into Remote Assist with the preview turned on.
- Taking multiple photos in succession can fail or be slow.
- Photos taken in Remote Assist have a limited resolution of 1280x720; lower than the maximum resolution available on the HoloLens.