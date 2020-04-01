---
author: sopsun
description: Remote Assist advanced deployment scenarios 
ms.author: sophiasysun
ms.date: 04/01/2020
ms.service: crm-online
ms.topic: article
title: Remote Assist advanced deployment scenarios 
ms.reviewer: krbjoran
---

# Dynamics 365 Remote Assist advanced deployment scenarios 

A Remote Assist call involves one party (technician) using Remote Assist and the other using Teams (expert or remote collaborator).  In most cases, technician and remote collaborators all belong to the same tenant, and thus a [standard deployment of Remote Assist](deploy-remote-assist.md) and [standard deployment of Teams](set-up-teams.md) is all you need. 

However, there are certain scenarios where this may not be the case: 

1. **Scenario 1: Multi-tenant company deployments,** i.e., a company has a multi-tenant configuration across different organizations or business units. 

1. **Scenario 2: Vendors and contractors using Remote Assist,** i.e., a company wants vendors and contractors that aren’t part of the company tenant to use Remote Assist.  

>[!NOTE]
> This article is intended for administrators, and assumes that you have Microsoft Teams **AND** Azure Active Directory (Azure AD) admin privileges. You should also be familiar with the [Teams admin portal](https://admin.teams.microsoft.com/).

## Account types

Throughout this article, we'll be referring to a few account types: 

1. **Internal account**: An Azure Active Directory (Azure AD) account that is created inside your tenant for internal users.
2. **Service account**: An Azure AD account that is created inside your tenant for users who are not currently part of your tenant.
3. **Guest account**: An Azure AD account that is created in your tenant when you "guest" any individual into a Teams team or channel using their email. 
    1. If that user's email is already associated with an Azure AD account in another tenant, that user is now part of 2 tenants: that user is a member of their native tenant and a guest in your tenant.
    2. If that user's email is not already associated with an Azure AD account in another tenant, that user is now part of 1 tenant: that user is a guest in your tenant.


## Scenario 1: Multi-tenant company deployments 

### Overview

In this scenario, a company leverages multiple tenants through different organizations and business units, all within the same company. One specific tenant (Tenant ABC) has experts that will provide support to one (or many) company employees that sit in a different tenant, as represented in the Figure 1.1.  

[!Note] This scenario only applies if all the tenants belong to the same company and the various tenants that need to use Remote Assist already have Remote Assist licenses. 

**Figure 1.1**
![Diagram showing tenant ABC needing to communicate with several external tenants.](media/cross-tenant-overview.png)

There are two solutions for this scenario: **Federation** and **Guesting**.

### Solution 1: Federation

**Federation** is a Microsoft Teams feature that allows other tenant domains to communicate with people in your tenant. There are three types of federation options: 

- Open federation
- "Allow specific" domains
- "Block specific" domains

>[!NOTE]
> See the Microsoft Teams [article on managing external access](https://docs.microsoft.com/microsoftteams/manage-external-access#plan-for-external-access) for more information.

In the following diagram example, tenants Contoso1, Contoso2, and ContosoN have their own Remote Assist licenses (which each come with Teams licenses). Tenant ABC has their own Teams licenses. (Please see Figure 1.2) 

**Figure 1.2**
![Diagram showing how the different tenants relate to one another.](media/cross-tenant-federation.png)

#### Federation pros and cons 

| Pros                                                                  | Cons                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Open federation is typically on by default.                           | Domain management may be more involved if not using open federation.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| If open federation is not enabled by default, it's easy to configure. | Open federation requires configuration on the additional tenants' side. The other tenants must either have open federation.                                                                                                                                                                                                                                                                                                                                                                                                           |
|                                                                       | Federation has fewer control features than guesting; when someone is guested into a Teams team, that user can only search and collaborate with people in the specific team they were guested into. When tenants are federated, everyone in each tenant can search and collabroate with everyone in other tenants. See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features. |

 >[!NOTE]
 >Tenant ABC and the external tenants do *not* have to have the same federation configuration. Tenant ABC can have open federation while the external tenants have "block" or "allow" federation settings.

 >[!NOTE]
 >If an external user wants to initiate a Remote Assist call with an expert in Tenant ABC, they will have to type out the entire email address of the expert in Tenant ABC. 

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

In the following diagram, the different company tenants (Contoso1, Contoso2, and ContosoN) have their own Remote Assist and Teams licenses. Tenant ABC has their own Teams licenses. Since in this case they are the remote collaborator, they don’t need a Remote Assist license. (Please see Figure 1.3) 

**Figure 1.3**
![Diagram showing external tenants and how they map to the internal tenant.](media/cross-tenant-guesting.png)

| Pros                                                                                                                                                                                                                                                                                                                                                                                                                                       | Cons                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| In this solution, Tenant ABC can guest in one (or more) individual external users instead of an entire external tenant.                                                                                                                                                                                                                                                                                                                    | May require more user management than with federation depending on the number of guests. |
| Guesting has more control features. For example, an external user is guested into a specific Teams teams and channels and can only search and collaborate with others who are inside the same Teams teams and channels. See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features |                                                                                          |

For more information, see this Microsoft Teams article about [how guest access works](https://docs.microsoft.com/en-us/microsoftteams/guest-access).

#### Guesting implementation

See this [Microsoft Teams guest access checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist) for full implementation instructions.


## Scenario 2: Vendors and contractors using Remote Assist

### Overview

> [!Note] To appropriately license this scenario, please contact your Microsoft sales representative to license.

Companies frequently want to leverage non-company employees such as vendors or contractors to perform specific service tasks. In this case, companies still handle all license configuration, but want to enable their vendors or contractors to seamlessly use Remote Assist to collaborate with them. 

### Example

Company ABC uses Tenant ABC. Tenant ABC has users who want to use Teams to remotely collaborate with company vendors and contractors. Some of these vendors and contractors are in an existing tenant and others are not. Company ABC wants to give vendors and contractors Remote Assist licenses so they can use it for their daily service tasks. This scenario is depicted in Figure 2.1 

In Figure 2.1, Company ABC used Azure AD to create **service accounts** (SAs) inside Tenant ABC. Tenant ABC administrator assigned a Remote Assist license (Jason - anything else?) to each service account. Service account credentials were then distributed to company vendors and contractors.
* Bob@Contoso1.com is still a member of Contoso1, and now uses SA1@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.
* Toni@Contoso1.com is still a member of ContosoN, and now uses SA2@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.
* User@Outlook.com was not a member of any other tenant - that contractor uses a regular personal email (e.g. @outlook.com) for work. Now, user@outlook.com users SA3@ABC.com to log in to Remote Assist to collaborate with Teams users in Tenant ABC.

**Figure 2.1**
![Diagram showing Tenant A providing a Remote Assist license to users outside of Tenant A.](media/cross-tenant-licensing.png)

[!Note] If Tenant ABC does not configure information barriers, any service account user can search for and communicate with any other service account user or internal account user in Tenant ABC. Learn more about information barriers and how to configure them [here](how-to-lease-ra.md).

[!Note] Because Teams users and Remote Assist users are all in Tenant ABC, they can each search for users they are allowed to search for by typing that user's name, rather than typing their entire email address.

### Implementation

If you are following the steps in the [Deploy HoloLens in a Commercial Environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

Otherwise, please learn how to [Provide Remote Assist licenses to users outside your tenant](how-to-lease-ra.md).

