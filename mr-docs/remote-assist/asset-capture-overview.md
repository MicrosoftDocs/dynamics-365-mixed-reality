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
Overview of what this is

## Entity Reference

Asset Capture utilizes several entities stored in Common Data Model:

1. Customer Asset: the individual asset.
2. Customer Asset Category: a way to describe a group of similar assets.
3. Customer Asset Attachment: individual media items captured in HoloLens of a single asset.
4. Account: the customer who owns the asset or it exists in their facility.
5. Product: the make/model of the asset

## Additional notes

- Support for HoloLens 1 and Mobile is not part of the June public preview and is **planned**.

### Known issues

- Users with access to a large number of environments will experience long delays the first time they sign into Remote Assist with the preview turned on.
- Taking multiple photos in succession can fail or be very slow.
- Photos taken in Remote Assist have a limited resolution of 1280x720; lower than the maximum resolution available on the HoloLens.