---
author: sophiasysun
description: Multi-tenant company deployments for Dynamics 365 Remote Assist
ms.author: sopsun
ms.date: 04/01/2020
ms.service: crm-online
ms.topic: article
title: Multi-tenant company deployments
ms.reviewer: krbjoran
---

# Multi-tenant company deployments

A Dynamics 365 Remote Assist call involves one party (technician) using Remote Assist and the other using Teams (expert or remote collaborator).  In most cases, technicians and remote collaborators all belong to the same tenant, and thus a [standard deployment of Remote Assist](deploy-remote-assist.md) and [standard deployment of Teams](set-up-teams.md) is all you need. 

However, there are certain scenarios where this may not be the case: 

1. **Multi-tenant company deployments** - a company has a multi-tenant configuration across different organizations or business units. This document focuses on this scenario.

2. **Vendors and contractors using Remote Assist** - a company wants vendors and contractors that aren’t part of the company tenant to use Remote Assist. [Learn more about this scenario](vendor-use-RA.md).

## Account types

Throughout this article, we'll be referring to a few account types: 

1. **Internal account**: An Azure Active Directory (Azure AD) account that is created in your tenant for internal users.
2. **Guest account**: An Azure AD account that is created in your tenant when you "guest" any individual into one or more Teams teams or channels using their email. 
    1. If that user's email is already associated with an Azure AD account in one other tenant, that user is now part of two tenants: that user is a member of their native tenant and a guest in your tenant.
    2. If that user's email is not already associated with an Azure AD account in any another tenant, that user is now part of one tenant: that user is a guest in your tenant.


## Scenario overview

In this scenario, which is represented in Figure 1.1, a company leverages multiple tenants through different organizations and business units, all within the same company. One specific tenant (Tenant ABC) has experts who will use Teams to provide support to one (or many) company employees that sit in a different company tenant (that is, Tenant Contoso1, Tenant Contoso2). 

Additional details:
- Each technician in Tenant Contoso1 and Tenant Contoso2 already has a Remote Assist license and Teams license.
- Each expert in Tenant ABC already has a Teams license. Experts who use Teams do not need a Remote Assist license. 
- Experts in Tenant ABC want to collaborate with technicians in Tenant Contoso1. 
- Experts in Tenant ABC also want to collaborate with technicians in Tenant Contoso2. 
- Technicians in Tenant Contoso1 do not want to search or collaborate with technicians in Tenant Contoso2.

>[!Note] 
> This scenario only applies if all the tenants belong to the same company and the various tenants that need to use Remote Assist already have Remote Assist licenses. 

**Figure 1.1**
![Diagram showing tenant ABC needing to communicate with several external tenants.](media/MultiTenant.png)

Now, Company ABC must set up **Federation** or **Guesting** to enable users in different tenants to collaborate with each other.

### Solution 1: Federation

[!NOTE] At this time, federation is only supported for calls with Remote Assist HoloLens users.

**Federation** is a Microsoft Teams feature that allows other tenant domains to communicate with people in your tenant. There are three types of federation options: 

- Open federation
- "Allow specific" domains
- "Block specific" domains

>[!NOTE]
> For more information, see the Microsoft Teams [article on managing external access](https://docs.microsoft.com/microsoftteams/manage-external-access#plan-for-external-access).

Figure 1.2 shows that Tenant ABC is federated with Tenant Contoso1, and Tenant ABC is also federated with Tenant Contoso2. Now, experts in Tenant ABC can search and collaborate with technicians in Contoso1. Experts in Tenant ABC can also search and collaborate with technicians in Contoso2. Technicians in Tenant Contoso1 cannot search or collaborate with technicians in Tenant Contoso2, and vice versa.

**Figure 1.2**
![Diagram showing how the different tenants relate to one another.](media/Federation.png)

#### Federation pros and cons 

| Pros                                                                  | Cons                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Open federation is typically on by default.                           | Domain management may be more involved if not using open federation.                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| If open federation is not enabled by default, it's easy to configure. | Open federation requires configuration on the additional tenants' side.                                                                                                                                                                                                                                                                                                                                                                                                            |
|                                                                       | Federation has fewer control features than guesting; when someone is guested into a Teams team, that user can only search and collaborate with people in the specific team they were guested into. When tenants are federated, everyone in each tenant can search and collaborate with everyone in other tenants. See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features. |

 >[!NOTE]
 >Tenants do *not* need to have the same federation configuration. Tenant ABC can have open federation while Tenant Contoso1 and Tenant Contoso2 have "block" or "allow" federation settings.

 >[!NOTE]
 >If an user wants to initiate a Remote Assist call with a collaborator outside their tenant, that user will need to type out the full email address of the collaborator outside their tenant.

#### Federation implementation

If you are following the steps in the [Deploy HoloLens in a commercial environment](https://docs.microsoft.com/hololens/hololens-requirements#apps) article, go back to that document before implementing this solution.

If you would like to implement **"Blocked"** or **"Allow"** Federation, see full instructions [here](https://docs.microsoft.com/microsoftteams/manage-external-access#allow-or-block-domains). 

To implement open federation, 

1. [Enable external access](https://docs.microsoft.com/microsoftteams/manage-external-access) in your Teams admin center. This allows users in your organization to make calls and chat with users outside your domain.

    ![Enable external access](media/enable-external-access.PNG "Enable external access")

    By default, users can communicate with users in any other domain that has external access turned on and that has allowed external access with your domain. If you want to restrict this behavior, you can add allowed or blocked domains. For more information, see [Manage external access (federation) in Microsoft Teams](https://docs.microsoft.com/microsoftteams/manage-external-access).

1. To check to see if a contact in another domain has external access enabled in their company’s Teams admin center, try typing the contact's full email address in Teams. When external access is allowed between both domains, Teams shows the following message:

    ![Confirmation message](media/access-enabled-confirmation.PNG "Confirmation message")

### Solution 2: Guesting

> [!NOTE]
> This solution is *not* necessary if one of the following is true:
>
> - Open federation is used.
> - Contoso1 or Contoso2 is on Tenant ABC's "allow" list.
> - Contoso1 or Contoso2 is off of Tenant ABC's "block" list.

Figure 1.3 shows the solution. Each tenant that has Remote Assist users who want to collaborate with Expert1@ABC.com and Expert2@ABC.com must guest each expert into a specific Teams team or channel. Then, that expert can only search and collaborate with other internal account users and guest account users in that team or channel.

**Figure 1.3**
![Diagram showing external tenants and how they map to the internal tenant.](media/Guesting.png)

| Pros                                                                                                                                                                                                                                                                                                                                                                                                                                       | Cons                                                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- |
| In this solution, Tenant Contoso1 and Tenant Contoso2 can each guest in one (or more) individual experts users instead of enabling collaboration with everyone in Tenant ABC.                                                                                                                                                                                             | May require more user management than with federation depending on the number of guests. |
| Guesting has more control features. For example, an external user is guested into a specific Teams teams and channels and can only search and collaborate with others who are inside the same Teams teams and channels. See [this article](https://docs.microsoft.com/microsoftteams/communicate-with-users-from-other-organizations#compare-external-and-guest-access) for a detailed comparison between guesting and federation features | The expert can only use Teams in one tenant at a time, which means that the expert can only communicate with technicians in a certain tenant if the technician is currently using Teams in that tenant. In our example, the expert is in a member in their native tenant (Tenant ABC), a guest in Tenant Contoso1, and a guest in Tenant Contoso2. To switch tenants, navigate to the top-right corner of Teams desktop app. To the left of your profile picture, you will see the name of the tenant you are currently in. Select it, and then select the tenant you'd like to switch to.  |

For more information, see this Microsoft Teams article about [how guest access works](https://docs.microsoft.com/microsoftteams/guest-access).

#### Guesting implementation

See this [Microsoft Teams guest access checklist](https://docs.microsoft.com/microsoftteams/guest-access-checklist) for full implementation instructions.
