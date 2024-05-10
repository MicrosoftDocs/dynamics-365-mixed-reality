---
author: davepinch
description: Multitenant company deployments for Dynamics 365 Remote Assist.
ms.author: davepinch
ms.date: 05/06/2024
ms.topic: conceptual
title: Multitenant company deployments
ms.reviewer: v-wendysmith
---

# Multitenant collaboration

[!INCLUDE [try-guides-ra](../includes/try-guides-ra.md)]

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

Learn about deploying a [multitenant collaboration](common-deployment-scenarios.md#scenario-2-multi-tenant-collaboration).

## Account types

There are two types of accounts:

- **Internal account**: A Microsoft Entra account that is created in your tenant for internal users.
- **Guest account**: A Microsoft Entra account that is created in your tenant when you provide an out-of-tenant user with guest access in one or more Teams teams or channels. You can "guest" an out-of-tenant user into your tenant using their email.
  - If that user's email is already associated with a Microsoft Entra account in one other tenant, that user is now part of two tenants: that user is a member of their native tenant and a guest in your tenant.
  - If that user's email isn't already associated with a Microsoft Entra account in any other tenant, that user is now part of one tenant: that user is a guest in your tenant.

## Scenario overview

In this scenario, a company uses multiple tenants through different organizations and business units, all within the same company. Teams users in Tenant ABC want to collaborate with Dynamics 365 Remote Assist users in Tenant Contoso1 and Tenant Contoso2.

In addition:

- Each technician in Tenant Contoso1 and Tenant Contoso2 already has a Dynamics 365 Remote Assist license and Teams license.
- Each expert in Tenant ABC already has a Teams license. Experts who use Teams don't need a Dynamics 365 Remote Assist license. 
- Teams users in Tenant ABC want to search and collaborate with Dynamics 365 Remote Assist users in Tenant Contoso1, and vice versa.
- Teams users in Tenant ABC want to search and collaborate with Dynamics 365 Remote Assist users in Tenant Contoso2, and vice versa.
- Remote Assist users in Tenant Contoso1 don't want to search or collaborate with Dynamics 365 Remote Assist users in Tenant Contoso2, and vice versa.

![Diagram showing tenant ABC needing to communicate with several external tenants.](media/MultiTenant.png)

Set up [**External access**](#solution-1-external-access-federation) or [**Guest access**](#solution-2-guest-access) to enable users in different tenants to collaborate with each other.

### Solution 1: External access (federation)

> [!NOTE]
> External access isn't supported for calls with Dynamics 365 Remote Assist mobile users.

**External access** is a Teams feature that allows Teams users from an entire external tenant to use Teams to find, call, chat, and set up meetings with users in your tenant. For more information, go to [Manage external access](/microsoftteams/manage-external-access).

There are three external access options:

- Open federation (default setting in Teams)
- Allow specific domains
- Block specific domains

In this example, Tenant ABC and Tenant Contoso1 enabled external access with each other. Tenant ABC and Tenant Contoso2 enabled external access with each other. Tenant Contoso1 and Tenant Contoso2 didn't enable external access with each other. Now:

- Teams users in Tenant ABC can search and collaborate with Dynamics 365 Remote Assist users in Tenant Contoso1, and vice versa.
- Teams users in Tenant ABC can search and collaborate with Dynamics 365 Remote Assist users in Tenant Contoso2, and vice versa.
- Dynamics 365 Remote Assist users in Tenant Contoso1 can't search or collaborate with Dynamics 365 Remote Assist users in Tenant Contoso2, and vice versa. If a user wants to initiate a Dynamics 365 Remote Assist call with a collaborator outside their tenant, that user must type out the full email address of the collaborator outside their tenant.

![Diagram showing how the different tenants relate to one another.](media/Federation.png)

#### External access pros and cons 

| Pros                                                                  | Cons                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Open federation is typically on by default.                           | Tenant management might be more involved if not using open federation.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| If open federation isn't enabled by default, it's easy for your tenant to configure. | Open federation requires configuration on the other tenants' side.                                                                                                                                                                                                                                                                                                                                                                                                            |
|                                                                       | External access has fewer control features than guest access. When you provide a user with guest access in a specific Teams team or channel, that user can only search and collaborate with people in that specific team or channel. When a tenant enables external access for another tenant, every user in each tenant can search and collaborate with every user in the other tenant. |
|                                                                       | External access enables fewer features than guest access. For example, when using external access, Dynamics 365 Remote Assist users and Teams users in different tenants can't join group calls with each other and can't share files with each other. For more information, go to [Compare external access and guest access](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access). |

 > [!NOTE]
 > Tenants *don't* need to have the same external access configuration. Tenant ABC can have **Open federation** while Tenant Contoso1 and Tenant Contoso2 have **Block** or **Allow** settings.

#### External access (federation) implementation

If you're following the steps in the [Deploy HoloLens in a commercial environment](/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution. Otherwise, go to [Manage external access](/microsoftteams/manage-external-access).

### Solution 2: Guest access

Guest access enables Teams admins or members to add individual users from outside their tenant into specific Teams teams and channels.

In this example, each tenant has guest access set up for a couple of experts. Each tenant that has Dynamics 365 Remote Assist users can collaborate with Expert1@ABC.com and Expert2@ABC.com in a specific Teams team or channel. Now:

- When Expert1@ABC.com uses Teams in Tenant ABC, Expert1@ABC.com can only search and collaborate with internal users and other guests in Tenant ABC. The same functionality applies to Expert2@ABC.com.
- When Expert1@ABC.com uses Teams in Tenant Contoso1, Expert1@ABC.com can only search and collaborate with internal users and other guests in Tenant Contoso1. The same functionality applies to Expert2@ABC.com.
- When Expert1@ABC.com uses Teams in Tenant Contoso2, Expert1@ABC.com can only search and collaborate with internal users and guests in Tenant Contoso2. The same functionality applies to Expert2@ABC.com.

> [!NOTE]
> Unlike Teams users, Dynamics 365 Remote Assist users can only use Dynamics 365 Remote Assist in one tenant. Thus, we do not recommend Teams users to guest Dynamics 365 Remote Assist users into the Teams users' tenant.

![Diagram showing external tenants and how they map to the internal tenant.](media/Guesting.png)

#### Guess access pros and cons

| Pros                                                                                                                                                                                                                                                                                                                                                                                                                                       | Cons                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| Tenant Contoso1 and Tenant Contoso2 can provide guest access to specific Teams users instead of enabling collaboration with everyone in Tenant ABC.                                                                                                                                                                                             | Compared to external access, guest access might require more user management. |
| Guest access offers more control features. For example, an out-of-tenant user who is a guest to a specific Teams team or channel can only search and collaborate with others who are inside the same Teams team or channel. For more information, go to [Compare external access and guest access](/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access). | A Teams user can only use Teams in one tenant at a time. The expert can only communicate with technicians in a certain tenant if the expert is currently using Teams in the technician's tenant. In our example, Expert1@ABC.com is in a member in their native tenant (Tenant ABC), a guest in Tenant Contoso1, and a guest in Tenant Contoso2. Expert1@ABC.com can only collaborate with technicians in Tenant Contoso1 if Expert1@ABC.com is using Teams in Tenant Contoso1. <br><br> To switch tenants in Teams desktop, select your profile picture, then select the tenant you'd like to switch to. <br><br> To switch tenants in Teams mobile, select the current tenant, then select the tenant you'd like to switch to. |

For more information, go to [Guest access in Teams](/microsoftteams/guest-access).

#### Guest access implementation

Go to [Collaborate with guests in a team](/microsoft-365/solutions/collaborate-as-team) for full implementation instructions.


[!INCLUDE[footer-include](../includes/footer-banner.md)]
