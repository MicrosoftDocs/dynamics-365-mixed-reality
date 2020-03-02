---
author: pawinfie
description:  Technical document for deploying cross-tenant/cross-company RA calls
ms.author: pawinfie
ms.date: 3/2/2020
ms.service: crm-online
ms.topic: article
title: Cross Tenant Communication
ms.reviewer:
---

# Remote Assist Cross Tenant Communication

## Who Is This Article For?

This Article is for Admins. This article assumes that you have Microsoft Teams admin privileges and are familiar with the [Teams Admin Portal](https://admin.teams.microsoft.com/)

## Account Types

The following terms will be used in this article:

1. Internal Account: An Azure AD account that is created inside of your company's tenant for internal users.
1. Service Account: An Azure AD account that is created inside of your company's tenant for external users. This account is exactly the same as an internal account. The only difference is that the account credentials are shared with users outside of your tenant/company.
1. Guest Account: An Azure AD account that sits outside of your company's tenant, but is "guested" into your tenant.

## Scenario 1: Communicating with Other Tenants

### One to Many Scenario Overview

In this scenario one tenant (Tenant ABC) has experts that will provide support to one (or many) customers. (See figure 1.1). There are two solutions for this scenario: Federation and Guesting.

**Figure 1.1**
![image](media/cross-tenant-overview.png)

### Solution 1: Federation

Federation is a Microsoft Teams feature that allows external domains to communicate with people in your organization. There are three types of federation options: Open Federation, "allow specific" domains, and "block specific" domains. Additional information is located [here](https://docs.microsoft.com/microsoftteams/manage-external-access#plan-for-external-access).

**Image 2.1**
![image](media/cross-tenant-federation.png)
In this image the external customers (Contoso1, Contoso2, and ContosoN) have their own Remote Assist license and Teams licenses. Tenant ABC have their own Teams licenses.

**Pros of Federation:**

1. Open Federation is typically on by default.

1. If Open Federation is not enabled by default, it is easy to configure.

**Cons of Federation:**

1. If Tenant ABC does not want to use open federation, Tenant ABC will have to manage the domains that are allowed to (or blocked from) communicating with them. However, editing domains is easy.

1. This solution requires configuration on the external tenants’ side. The external tenants has to either have Open Federation, add Tenant ABC’s domain to their “allow” list, or ensure that Tenant ABC’s domain is not on their “blocked” list.
    >[!NOTE]
    >Tenant ABC and the external tenants do **NOT** have to have the same federation configuration. Tenant ABC can have Open Federation while the external tenants have "block"/"allow" federation settings.

1. If an external user wants to initiate a Remote Assist call with an expert in Tenant ABC, they will have to type out the entire email address of the expert in Tenant ABC.

1. This solution grants all users on the external tenant(s) the ability to call/chat with anyone in Tenant ABC.

1. Federation has less control features. A detailed comparison between Guesting and Federation features is located [here]( https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access).

#### Federation Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

Instructions on implementing **Open Federation** are located [here](cross-company-calling.md).

Instructions for implementing **Blocked/Allow Federation** are located [here](https://docs.microsoft.com/microsoftteams/manage-external-access#allow-or-block-domains).

### Solution 2: Guesting

> [!NOTE]
> This solution is **NOT** necessary if one of the following is true: Open Federation is used, if the external tenant is on Tenant ABC’s “allow” list, or if the external tenant is off of Tenant ABC’s “block” list.

**Image 3.1**
![image](media/cross-tenant-guesting.png)

In this image the external customers (Contoso1, Contoso2, and ContosoN) have their own Remote Assist license. Tenant ABC have their own Teams licenses.

**Pros of Guesting:**

1. In this solution, Tenant ABC can guest in one (or more) external users instead of an entire external tenant.

1. Guesting has more control features. A comparison between Guesting and Federation features is located [here]( https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access).

**Cons of Guesting:**

1. May require more managing of users than with Federation.

1. This solution grants guested users the ability to call/chat with anyone in Tenant ABC.
To learn more about guesting, visit [here]( https://docs.microsoft.com/microsoftteams/guest-access).

To learn more about guesting, visit [here]( https://docs.microsoft.com/microsoftteams/manage-external-access).

#### Guesting Implementation

Instructions on implementing **Guesting** are located [here](https://docs.microsoft.com/microsoftteams/guest-access-checklist)

## Scenario 2: Leasing Services to Other Tenants

### Scenario Overview

In this scenario, one tenant (Tenant ABC) has experts that will provide support to one (or many) customers. Tenant ABC wants to lease out a Remote Assist License to the tenants they support. Please see Figure 4.1.

**Figure 4.1**
![image](media/cross-tenant-licensing.png)

In this figure Tenant ABC assigns unique service accounts to external tenants. For example: SA1 is given to a user (or multiple users) in Contoso1, SA2 is given to Contoso2, and so forth.
>[!NOTE]
> Tenant ABC can give multiple services accounts to an external tenant.

### Solution

Tenant ABC will need to create “Service accounts” in Azure AD. These accounts are then distributed to users in external Tenants.

**Pros:**

1. Tenant ABC can assign RA licenses (and other licenses if necessary) to their customers on external tenants.

1. Tenant ABC can control who the external users - who are using the Service Accounts - can communicate with. This can be accomplished with the implementation of information barrier policies.

1. If an external users wants to initiate a Remote Assist call with an expert in Tenant ABC, they are able to search for the user without typing that user’s entire email address.

**Cons:**

1. Depending on how many customers Tenant ABC has, Tenant ABC may need to create/manage many service accounts.

1. External users can search for and communicate with anyone in the organization if Information Barriers are not in place.

#### Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, please go back to that document before implementing this solution.

Instructions on implementing are located [here](cross-tenant-licensing-implementation.md).