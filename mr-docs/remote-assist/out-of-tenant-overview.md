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

A Remote Assist call involves one party (technician) using Remote Assist and the other using Teams (expert or remote collaborator).  In most cases, technician and remote collaborators all belong to the same tenant, and thus a standard deployment of Remote Assist (deploy-remote-assist.md) and Teams (set-up-teams.md) is all you need. 


However, there are certain scenarios where this may not be the case: 

Scenario 1: Vendors and contractors using Remote Assist, i.e., a company wants vendors and contractors that aren’t part of the company tenant to use Remote Assist.  
Scenario 2: Multi-tenant company deployments, i.e., a company has a multi-tenant configuration across different organizations or business units. 

This document explains ...

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

## Scenario 1: Vendors and contractors using Remote Assist

> [!Note] This section assumes that vendors and contractors are not part of your company. 
>
> If vendors are part of a different tenant in your company and *you* would like to configure Remote Assist licenses for them, you may license this scenario without contacting your Microsoft sales representative.
> 
> If vendors are part of a different tenant in your company and *they* would like to configure Remote Assist licenses, the vendor tenant's administrator should do a standard deployment of Remote Assist (deploy-remote-assist.md). Then, your tenant needs to set up federation with the vendor tenant.

> [!Note] This section assumes the vendors and contractors do not have Remote Assist licenses. If the vendors have Remote Assist licenses in their own tenant (i.e. not in your tenant), you will need to use federation or guesting to enable experts in your tenant to collaborate with vendors in the vendor tenant.

### Scenario 1: Vendors and contractors using Remote Assist - Overview

[!Note] To appropriately license this scenario, please contact your Microsoft sales representative to license.

Companies frequently want to leverage non-company employees such as vendors or contractors to perform specific service tasks. In this case, companies still handle all license configuration, but want to enable their vendors or contractors to seamlessly use Remote Assist to collaborate with them. 

### Scenario 1: Vendors and contractors using Remote Assist - Example

The following example is depicted in Figure 2.1.

Company ABC uses Tenant ABC. Tenant ABC has users who want to use Teams to remotely collaborate with company vendors and contractors. Some of these vendors and contractors are in an existing tenant and others are not. Company ABC wants to give vendors and contractors Remote Assist licenses so they can use it for their daily service tasks. 

In Figure 2.1, Tenant ABC administrator used Azure AD to create **service accounts** (SAs) inside Tenant A. Tenant A administrator assigned a Remote Assist license (Jason - anything else?) to each service account. Service account credentials were then distributed to company vendors and contractors.
* Bob@Contoso1.com is still a member of Contoso1, and now uses SA1@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.
* Toni@Contoso1.com is still a member of ContosoN, and now uses SA2@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.
* User@Outlook.com was not a member of any other tenant - that contractor uses a regular personal email (e.g. @outlook.com) for work. Now, user@outlook.com users SA3@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.

**Figure 2.1**
![Diagram showing Tenant A providing a Remote Assist license to users outside of Tenant A.](media/cross-tenant-licensing.png)

[!Note] If Tenant ABC does not configure information barriers, any service account user can search for and communicate with any other service account user or internal account user in Tenant ABC. Learn more about information barriers and how to configure them [here](how-to-lease-ra.md).

[!Note] Because Teams users and Remote Assist users are all in Tenant ABC, they can each search for users they are allowed to search by searching that user's name, rather than searching their entire email address.

### Scenario 1: Vendors and contractors using Remote Assist - Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

Otherwise, please learn how to [Provide Remote Assist licenses to users outside your tenant](how-to-lease-ra.md).










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

