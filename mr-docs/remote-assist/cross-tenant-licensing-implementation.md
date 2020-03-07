---
author: pawinfie
description:  Technical document for deploying cross-tenant or cross-company Remote Assist calls
ms.author: pawinfie
ms.date: 03/06/2020
ms.service: crm-online
ms.topic: article
title: Cross-tenant Remote Assist licensing implementation
ms.reviewer: krbjoran
---

# Cross-tenant Remote Assist licensing implementation

>[!Note] 
> This article assumes that you have read the article [Remote Assist cross-tenant communication](cross-tenant-overview.md). If you haven't, please review that article first.

In this article, we'll take a look at how to implement licensing across multiple Remote Assist tenants through the following steps: 

1. Determine if information barriers are necessary
2. Buy the correct licenses
3. Configure information barriers

## Step 1. Determine if information barriers are necessary

Information barriers are a great way to control who can communicate with one another in Microsoft Teams. Information barriers use attributes to segment Azure Active Directory users. The segmentation of users determines which users can talk to one another.

It's important to plan how users will be segmented. For example, you may choose to segment users based on the attribute "Groups." Information barriers are then placed on the "Group" attribute to allow Group A to communicate with Group B but not with Group C.

>[!Note]
> To learn more about information barriers, see the following docs:
> - [Overview of information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide).
> - [Overview of segmentation and attributes](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-attributes?view=o365-worldwide).

If you want to control who the "Service Account" holders can communicate with, follow the **"Information Barrier Steps"** in each of the following sections. If controlling the communication between service account users and other users is not important for your organization, follow the **Normal steps** in each of the following sections.

## Step 2. Buy the correct licenses

### Information barrier steps

In order for information barriers to work, an information barrier license is required. The following licensing suites include information barrier licenses: 

- Microsoft 365 E5
- Office 365 E5
- Office 365 Advanced Compliance
- Microsoft 365 E5 Information Protection and Compliance

>![!Note]
> For more information, see: [Updated list of Information Barrier licenses](https://docs.microsoft.com/microsoft-365/compliance/information-barriers?view=o365-worldwide#required-licenses-and-permissions)


You'll also need the licenses for:

- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis#who-uses-azure-ad)
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams

### Normal steps

The following licenses are required:

- [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis#who-uses-azure-ad)
- [Remote Assist](buy-remote-assist.md)
- Microsoft Teams


>[!Note]
> If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

## Step 3. Configure information barriers

Finally, you'll need to configure the information barriers. Visit [this article on information barriers](https://docs.microsoft.com/microsoft-365/compliance/information-barriers-policies?view=o365-worldwide) for full instructions.

