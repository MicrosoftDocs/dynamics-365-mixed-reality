---
author: pawinfie
description:  Technical document for deploying cross-tenant or cross-company Remote Assist calls
ms.author: pawinfie
ms.date: 03/06/2020
ms.service: crm-online
ms.topic: article
title: Cross Tenant Communication
ms.reviewer: krbjoran
---

# Remote Assist cross-tenant communication

>[!Note]
> This article is intended for admins, and assumes that you have Microsoft Teams admin privileges. You should also be familiar with the [Teams admin portal](https://admin.teams.microsoft.com/).

## Account Types

Throughout this article, we'll be referring to a few types of accounts:

1. **Internal account**: An Azure Active Directory (AD) account that is created inside of your company's tenant for *internal* users.
2. **Service account**: An Azure AD account that is created inside of your company's tenant for *external* users.
3. **Guest account**: An Azure AD account that sits outside of your company's tenant, but is "guested" into your tenant.

## Scenario 1: Communicating with other tenants

### One-to-many 

In this scenario, one tenant (Tenant ABC) has experts that will provide support to one (or many) customers, as represented in the following diagram. 

![Diagram showing tenant ABC needing to communicate with several external tenants.](media/cross-tenant-overview.png)

There are two solutions for this scenario: **Federation** and **Guesting**.

### Solution 1: Federation

**Federation** is a Microsoft Teams feature that allows external domains to communicate with people in your organization. There are three types of federation options: 

- Open federation
- "Allow specific" domains
- "Block specific" domains
 
>[!Note]
> See the Microsoft Teams [article on managing external access](https://docs.microsoft.com/microsoftteams/manage-external-access#plan-for-external-access) for more information.

In the following diagram example, the external customers (Contoso1, Contoso2, and ContosoN) have their own Remote Assist license and Teams licenses. Tenant ABC has their own Teams licenses.
![Diagram showing how the different tenants relate to one another.](media/cross-tenant-federation.png)

#### Pros of federation

1. Open federation is typically on by default.

2. If open federation is not enabled by default, it's easy to configure.

#### Cons of federation

1. If Tenant ABC does not want to use open federation, Tenant ABC will have to manage the domains that are allowed to (or blocked from) communicating with them. However, editing domains is easy.

2. Open federation requires configuration on the external tenants’ side. The external tenants must either have open federation, add Tenant ABC’s domain to their “allow” list, or ensure that Tenant ABC’s domain is not on their “blocked” list.
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
> - Open federation is used, 
> - The external tenant is on Tenant ABC’s “allow” list.
> - The external tenant is off of Tenant ABC’s “block” list.

In the following diagram, the external customers (Contoso1, Contoso2, and ContosoN) have their own Remote Assist licenses. Tenant ABC has their own Teams licenses.

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

## Scenario 2: Leasing services to other tenants

### Scenario Overview

In this scenario, one tenant (Tenant ABC) has experts that will provide support to one (or many) customers. Tenant ABC wants to lease out a Remote Assist license to the tenants they support. Let's see what this looks like in a diagram: 

![Diagram showing an internal tenant leasing out a Remote Assist license to external tenants.](media/cross-tenant-licensing.png)

In this figure, Tenant ABC assigns unique service accounts to external tenants. For example: SA1 is given to a user (or multiple users) in Contoso1, SA2 is given to Contoso2, and so forth.
>[!NOTE]
> Tenant ABC can give multiple service accounts to an external tenant.

Tenant ABC will need to create “Service accounts” in Azure AD. These accounts are then distributed to users in external Tenants.

#### Pros of leasing services to other tenants

1. Tenant ABC can assign Remote Assist licenses (and other licenses if necessary) to their customers on external tenants.

2. Tenant ABC can control who the external users - who are using the service accounts - can communicate with. This can be accomplished with the implementation of information barrier policies.

3. If an external user wants to initiate a Remote Assist call with an expert in Tenant ABC, they are able to search for the user without typing that user’s entire email address.

#### Cons of leasing services to other tenants

1. Depending on how many customers Tenant ABC has, Tenant ABC may need to create and manage many service accounts.

1. External users can search for and communicate with anyone in the organization if information barriers are not in place.

#### Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

See our article on [cross-tenant licenscing](cross-tenant-licensing-implementation.md).