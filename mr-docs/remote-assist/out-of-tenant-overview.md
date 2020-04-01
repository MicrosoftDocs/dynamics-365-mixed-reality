---
author: sopsun
description:  Technical document for deploying cross-tenant or cross-company Remote Assist calls
ms.author: sophiasysun
ms.date: 04/01/2020
ms.service: crm-online
ms.topic: article
title: Using Remote Assist to collaborate with people outside your tenant 
ms.reviewer: krbjoran
---

# Using Remote Assist to collaborate with people outside your tenant 

A Remote Assist call involves one party using Remote Assist and the other using Teams. If the people who want to use Remote Assist and the people who want to use Teams are in the same tenant, you do not need to configure cross-tenant communication and you do not need to read this document.

This document describes 2 scenarios.

| Scenario                                                                                                                                                                           | Implementation overview                                                                                                                                                                                           |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Scenario 1: Remote collaborators in Tenant A want to use Teams, and technicians in Tenant B want to use Remote Assist. Technicians in Tenant B do not have Remote Assist licenses. | Tenant A administrator must set up service accounts in Tenant A, assign a Remote Assist license to each service account, and provide service account credentials to the technicians in Tenant B. Learn more here. |
| Scenario 2: Remote collaborators in Tenant A want to use Teams, and technicians in Tenant B want to use Remote Assist. Users in both tenants have the licenses they need.          | Tenant A and Tenant B must agree on how to enable users in the two tenants to communicate with each other: federation or guesting. Learn more here.                                                               |


>[!NOTE]
> This article is intended for administrators, and assumes that you have Microsoft Teams **AND** Azure Active Directory (Azure AD) admin privileges. You should also be familiar with the [Teams admin portal](https://admin.teams.microsoft.com/).

## Account types

Throughout this article, we'll be referring to a few account types: 

1. **Internal account**: An Azure Active Directory (Azure AD) account that is created inside your tenant for internal users.
2. **Service account**: An Azure AD account that is created inside your tenant for users who are not currently part of your tenant.
3. **Guest account**: An Azure AD account that is created in your tenant when you "guest" any individual into a Teams team or channel using their email. 
    1. If that user's email is already associated with an Azure AD account in another tenant, that user is now part of 2 tenants: that user is a member of their native tenant and a guest in your tenant.
    2. If that user's email is not already associated with an Azure AD account in another tenant, that user is now part of 1 tenant: that user is a guest in your tenant.

## Scenario 2: Providing Remote Assist licenses to users outside your tenant 

### Scenario 2 Overview

[@HGT, could you help me phrase this properly?] Companies frequently want to purchase Remote Assist licenses not because their own technicians need to use Remote Assist to get help, but because they want to provide Remote Assist licenses to their customers and provide best-in-class customer service. Companies want to handle all the license configuration and enable their customers to seamlessly use Remote Assist. 

[!Note]: To appropriately license this scenario if people who want to use Remote Assist are outside your company, please contact your Microsoft sales representative to license.

### Scenario 2 example

The following example is depicted in Figure 2.1.

Tenant A has remote collaborators who will use Microsoft Teams to assist technicians. Some technicians are in Tenant B, some technicians are in Tenant C, and others are not in any tenant.  

In Figure 2.1, Tenant A administrator created **service accounts** (SAs) inside Tenant A. Tenant A administrator assigned a Remote Assist license (Jason - anything else?) to each service account. Service account credentials were then distributed to the people outside Tenant A who want to use Remote Assist. More specifically,
* SA1 was given to a user (or multiple users who are sharing the SA1 account) who is currently a member of Tenant B
* SA2 was given to a user (or multiple users who are sharing the SA2 account) who is currently a member of Tenant C
* SA3 was given to a user who is not currently a member of any tenant

**Figure 2.1**
![Diagram showing Tenant A providing a Remote Assist license to users outside of Tenant A.](media/cross-tenant-licensing.png)

#### Pros of providing service accounts for users outside your tenant

1. Tenant A can assign Remote Assist licenses (and other licenses if necessary) to  customers on external tenants.

2. Tenant ABC can control who the external users - who are using the service accounts - can communicate with. This can be accomplished with the implementation of information barrier policies.

3. If an external user wants to initiate a Remote Assist call with an expert in Tenant ABC, they are able to search for the user without typing that user's entire email address.

#### Cons of providing service accounts for users outside your tenant

1. Depending on how many customers Company ABC has, Tenant ABC may need to create and manage many service accounts.

1. External users can search for and communicate with anyone in the Tenant ABC if Company ABC does not configure information barriers.

#### Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

Otherwise, please read [How to provide Remote Assist Licenses to External Users](cross-tenant-licensing-implementation.md).








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

1. In this solution, Tenant ABC can guest in one (or more) individual external users instead of an entire external tenant. 

2. Guesting has more control features. For example, an external user is guested into a specific Teams teams and channels and can only search and collaborate with others who are inside the same Teams teams and channels.  See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features.

#### Cons of guesting

1. May require more user management than with federation.

For more information, see this Microsoft Teams [article on granting guess access](https://docs.microsoft.com/microsoftteams/guest-access).

#### Guesting implementation

See this [Microsoft Teams guest access checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist) for full implementation instructions.

