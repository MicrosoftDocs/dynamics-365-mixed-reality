---
author: pawinfie
description:  Technical document for deploying cross-tenant or cross-company Remote Assist calls
ms.author: pawinfie
ms.date: 03/24/2020
ms.service: crm-online
ms.topic: article
title: Cross Tenant Communication
ms.reviewer: krbjoran
---

# Remote Assist external collaboration scenarios

A Remote Assist call involves one party using Remote Assist and the other using Teams. If the Remote Assist and Teams user are in the same tenant, you do not need to configure cross-tenant communication.

However, if you want to collaborate with someone outside of your tenant, there are two main scenarios that are covered in this article:

1. [Collaborating with someone outside of your tenant who has their own Remote Assist license.](#scenario-1-communicating-with-external-users)
1. [Leasing a Remote Assist license to someone outside of your tenant](#scenario-2-leasing-remote-assist-licenses-to-external-users)

>[!NOTE]
> This article is intended for admins, and assumes that you have Microsoft Teams **AND** Azure Active Directory (Azure AD) admin privileges. You should also be familiar with the [Teams admin portal](https://admin.teams.microsoft.com/).

## Account types

Throughout this article, we'll be referring to a few types of accounts:

1. **Internal account**: An Azure Active Directory (Azure AD) account that is created inside of your company's tenant for *internal* users.
2. **Service account**: An Azure AD account that is created inside of your company's tenant for *external* users.
3. **Guest account**: An Azure AD account that sits outside of your company's tenant, but is "guested" into your tenant.

## Scenario 1: Communicating with external users

### Scenario 1 overview

In this scenario, one tenant (Tenant ABC) has experts that will provide support to one (or many) customers, as represented in the Figure 1.1.

**Figure 1.1**
![Diagram showing tenant ABC needing to communicate with several external tenants.](media/cross-tenant-overview.png)

There are two solutions for this scenario: **Federation** and **Guesting**.

### Solution 1: Federation

**Federation** is a Microsoft Teams feature that allows external domains to communicate with people in your organization. There are three types of federation options:

- Open federation
- "Allow specific" domains
- "Block specific" domains

>[!NOTE]
> See the Microsoft Teams [article on managing external access](https://docs.microsoft.com/microsoftteams/manage-external-access#plan-for-external-access) for more information.

In the following diagram example, the external customers (Contoso1, Contoso2, and ContosoN) have their own Remote Assist license and Teams licenses. Tenant ABC has their own Teams licenses. (Please see figure 1.2)

**Figure 1.2**
![Diagram showing how the different tenants relate to one another.](media/cross-tenant-federation.png)

#### Pros of federation

1. Open federation is typically on by default.

2. If open federation is not enabled by default, it's easy to configure.

#### Cons of federation

1. If Tenant ABC does not want to use open federation, Tenant ABC will have to manage the domains that are allowed to (or blocked from) communicating with them. However, editing domains is easy.

2. Open federation requires configuration on the external tenants' side. The external tenants must either have open federation, add Tenant ABC's domain to their "allow" list, or ensure that Tenant ABC's domain is not on their "blocked" list.
    >[!NOTE]
    >Tenant ABC and the external tenants do *not* have to have the same federation configuration. Tenant ABC can have open federation while the external tenants have "block" or "allow" federation settings.

3. If an external user wants to initiate a Remote Assist call with an expert in Tenant ABC, they will have to type out the entire email address of the expert in Tenant ABC.

4. This solution grants all users on the external tenant(s) the ability to call/chat with anyone in Tenant ABC.

5. Federation has fewer control features. See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features.

#### Federation implementation

If you are following the steps in the [Deploy HoloLens in a commercial environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

- See [this article](cross-company-calling.md) for full instructions on implementing **open federation**.

- See [this Microsoft Teams article](https://docs.microsoft.com/microsoftteams/manage-external-access#allow-or-block-domains) for full instructions for implementing **"Blocked" and "Allow" Federation**.

### Solution 2: Guesting

> [!NOTE]
> This solution is *not* necessary if one of the following is true:
>
> - Open federation is used.
> - The external tenant is on Tenant ABC's "allow" list.
> - The external tenant is off of Tenant ABC's "block" list.

In the following diagram, the external customers (Contoso1, Contoso2, and ContosoN) have their own Remote Assist and Teams licenses. Tenant ABC has their own Teams licenses. (Please see Figure 1.3)

**Figure 1.3**
![Diagram showing external tenants and how they map to the internal tenant.](media/cross-tenant-guesting.png)

#### Pros of guesting

1. In this solution, Tenant ABC can guest in one (or more) external users instead of an entire external tenant.

2. Guesting has more control features.  See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features.

#### Cons of guesting

1. May require more user management than with federation.

2. This solution grants guested users the ability to call or chat with anyone in Tenant ABC.

For more information, see this Microsoft Teams [article on granting guess access](https://docs.microsoft.com/microsoftteams/guest-access).

#### Guesting implementation

See this [Microsoft Teams guest access checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist) for full implementation instructions.

## Scenario 2: Leasing Remote Assist licenses to external users

### Scenario 2 Overview

Companies frequently want to purchase Remote Assist licenses not because their own technicians need to use Remote Assist to get help, but because they want to give Remote Assist licenses to their customers to provide best-in-class customer service. Companies want to handle all the administrative set up and enable their customers to use Remote Assist licenses.

### Scenario 2 example

Company ABC has experts that will use Microsoft Teams to provide customer support to one (or many) customers. To do so, Company ABC will provide their customers with a Remote Assist license. This scenario is depicted in Figure 2.1.

In Figure 2.1, Company ABC created "Service accounts" (SAs) in Azure AD. These accounts were then distributed to external users. For example: SA1 was given to a user (or multiple users who are sharing the SA1 account) in the Contoso1 Tenant, SA2 was given to a user (or multiple users who are sharing the SA2 account) ContosoN Tenant, and SA3 was given to a user who does not belong to a tenant.

>[!NOTE]
> Service accounts can be given to anyone. The user receiving the service account does not have to belong to a Tenant.

**Figure 2.1**
![Diagram showing an internal tenant leasing out a Remote Assist license to external tenants.](media/cross-tenant-licensing.png)

#### Pros of leasing services to other tenants

1. Tenant ABC can assign Remote Assist licenses (and other licenses if necessary) to their customers on external tenants.

2. Tenant ABC can control who the external users - who are using the service accounts - can communicate with. This can be accomplished with the implementation of information barrier policies.

3. If an external user wants to initiate a Remote Assist call with an expert in Tenant ABC, they are able to search for the user without typing that user's entire email address.

#### Cons of leasing services to other tenants

1. Depending on how many customers Tenant ABC has, Tenant ABC may need to create and manage many service accounts.

1. External users can search for and communicate with anyone in the organization if information barriers are not in place.

#### Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

[How to Lease Remote Assist Licenses to External Users](cross-tenant-licensing-implementation.md).
