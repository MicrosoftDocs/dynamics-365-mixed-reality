---
author: pawinfie
description:  Technical document for deploying cross-tenant/cross-company RA calls
ms.author: pawinfie
ms.date: 2/26/2020
ms.service: crm-online
ms.topic: article
title: Cross Tenant Licensing Implementation Steps
ms.reviewer:
---

# Cross Tenant RA Licensing Implementation Steps

This document assumes that you have read the [Remote Assist Cross Tenant Communication](cross-tenant-overview.md). If you have not, please review that document first.

## Overview of Steps

1. [Determine if Information Barriers are Necessary](#step-1-determine-if-information-barriers-are-necessary)
1. [Buy the Correct Licenses](#step-2-buy-the-correct-licenses)
1. [Configure Information Barriers](#step-3-configure-information-barriers)

## Step 1. Determine if Information Barriers are Necessary

Information Barriers are a great way to control who can communicate with one another in Microsoft Teams. Information Barriers use attributes to segment Azure AD users. The segmentation of users determines which users can talk to one another. Because of this, it is extremely important to plan how users will be segmented. For example, you may choose to segment users based on the attribute "Groups". Information Barriers are then placed on the "Group" attribute to allow Group A to communicate with Group B but not with Group C.

- [Overview of Information Barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide).
- [Overview of segmentation and attributes](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide).

If you want to control who the "Service Account" holders can communicate with, follow the **"Information Barrier Steps"** in each of the following sections. If controlling the communication between service account users and other users is not important for your organization, follow the **"NORMAL STEPS"** in each of the following sections.

## Step 2. Buy the Correct Licenses

### Information Barrier Steps

In order for Information Barriers to work, an Information Barrier licenses is required. The following licensing suites include Information Barrier Licenses. ([Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)).

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

In addition, the following licenses are required:

- Azure Active Directory (Azure AD)
    >[!NOTE]
    > Azure AD licenses may come with the licenses listed above.
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams

### Normal Steps

The following licenses are required:

- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis#who-uses-azure-ad)
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams

### Jump Back to Articles

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

## Step 3. Configure Information Barriers

Information barrier steps can be found [here](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide).


