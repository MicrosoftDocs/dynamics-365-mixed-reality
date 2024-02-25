---
author: davepinch
description: Learn how to use Dynamics 365 Guides US Government for government organizations.
ms.author: davepinch
ms.date: 02/14/2024
ms.topic: overview
title: Dynamics 365 Guides US Government
ms.reviewer: v-wendysmith
---

# Dynamics 365 Guides US Government

In response to the unique and evolving requirements of the United States public sector, Microsoft has created Dynamics 365 Guides US Government, a plan for US government organizations. We recommend that you read this supplementary section alongside the [Guides documentation](./overview.md).

At this time, Dynamics 365 Guides US Government is offered only at the Government Community Cloud (GCC) level. It's currently unavailable for GCC High, and for the Department of Defense (DoD).  

The Dynamics 365 Guides US Government service description is designed to serve as an overlay to the general Dynamics 365 Guides service description. It defines the unique commitments of this service and the differences from Dynamics 365 Guides offerings.

## About the Dynamics 365 Guides US Government GCC plan environment

The Dynamics 365 Guides US Government GCC plan (referred to as "the GCC plan" or "GCC environment" in the rest of this article) is a monthly subscription that can be licensed to an unlimited number of users.

The GCC environment provides compliance with federal requirements for cloud services, including Federal Risk and Authorization Management Program (FedRAMP) moderate, CJIS, IRS 1075, and DISA SRG L2 requirements.

In addition to the features and capabilities of Dynamics 365 Guides, organizations that use the GCC plan benefit from the following unique features:

- Your organization’s customer content is stored within the United States.

- Access to your organization’s customer content is restricted to [screened Microsoft personnel](/power-platform/admin/microsoft-dynamics-365-government#restricted-data-access-by-administrators).

- The GCC plan is designed to comply with certifications and accreditations that are required for US public sector customers with FedRAMP moderate requirements.

Copy API isn't available in the GCC environment.

## Customer eligibility

The GCC plan is available to: (1) US federal, state, local, tribal, and territorial government entities; (2) Other entities that handle data that is subject to government regulations and requirements and where use of the GCC plan is appropriate to meet these requirements, subject to validation of eligibility. Validation of eligibility by Microsoft includes confirmation of handling law enforcement data subject to the FBI's Criminal Justice Information Services (CJIS) policy, or other government-regulated or controlled data. Validation might require sponsorship by a government entity with specific requirements for the handling of data.

Entities with questions about eligibility for the GCC plan should consult their account team. Upon renewal of a customer's contract for the GCC plan, revalidation of eligibility is required.

## Availability and access to the GCC plan

Access to the GCC plan is offered as a monthly subscription and can be licensed to an unlimited number of users.

The GCC plan is available through the Volume Licensing and Cloud Solution Provider purchasing channels. 

## What is customer data and customer content?

Customer data, as defined in the Online Services Terms, means all data, including all text, sound, video, 3D objects, or image files, and software that are provided to Microsoft by or on behalf of, customers through the use of the Online Service. Customer content refers to a specific subset of customer data that has been directly created by users, such as content stored in databases through entries in [Microsoft Dataverse](/powerapps/maker/common-data-service/data-platform-intro) entities (for example, 3D objects). Content is generally considered confidential information and in normal service operation isn't sent over the internet without encryption.

Microsoft reminds you not to share any controlled, sensitive, or confidential information with support personnel as part of your GCC-related support incident, until you confirm their authorization to view or access such data. Microsoft is committed to protecting your privacy. Dynamics 365 Guides Customer Support isn't included in the service accreditation boundary and doesn't provide FedRAMP, CJIS, IRS 1075, DISA SRG L2 data handling and/or compliance assurances.

For more information on Dynamics 365 Guides protection of customer data, see the [Microsoft Online Services Trust Center](https://www.microsoft.com/en-us/trust-center/product-overview). 

## Customer content located within the United States

GCC plan services are provided from datacenters physically located in the United States. GCC plan customer content is stored at rest in datacenters physically located only in the United States.

## Guest access and the GCC environment

If you try to [invite a guest user](admin-add-guest-user.md) who isn't in the same government cloud, you'll see the following error message:

>[!CAUTION]
>_"The user you are inviting does not exist in this national cloud. To collaborate with this user, ask them for a different email address associated with the directory in this national cloud or create User Account for them in Microsoft Entra"._

For more info, see [⁠Microsoft Entra B2B in government and national clouds](/azure/active-directory/external-identities/b2b-government-national-clouds).

[!INCLUDE [azure-ad-to-microsoft-entra-id](../includes/azure-ad-to-microsoft-entra-id.md)]

[!INCLUDE[footer-include](../includes/footer-banner.md)]
