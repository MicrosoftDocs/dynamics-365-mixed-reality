---
title: Prerequisites for implementation and rollout
description: Learn the prerequisites before you implement Dynamics 365 Guides in a regulated industry, and to help plan the rollout of the solution.
ms.date: 03/09/2023
ms.topic: conceptual
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Prerequisites for implementation and rollout

As prerequisites for a successful Dynamics 365 Guides rollout in regulated industries, we recommend that you define the following elements in the initial phases of the implementation:

- The Guides user journey
- The data model
- System integrations and reuse
- Notifications

Consider these four elements early in the process, because they have significant influence on the overall implementation process and the possibilities for future development.

## The Guides user journey

We recommend that you facilitate a series of internal stakeholder workshops for employees with standard operating procedure (SOP) touchpoints. The group of stakeholders should include, but isn't limited to, SOP authors, digital training consultants, business and IT quality assurance (QA) specialists, Microsoft Power Platform personnel from IT, and operators.

The purpose of the workshops is to receive stakeholder input about the relevant steps and roles that are involved from the creation of a guide until it's archived, and to identify potential pain points in the life cycle. When this information is mapped in a detailed user journey, it helps you design the right environment structure and the flow of guides between environments, and select the right roles to associate with each environment. It also helps you identify existing systems that your organization can take advantage of and processes that your organization can reuse or simplify.

## The data model

A data model provides a blueprint that shows where data comes from, what format it's in, how it's stored and accessed, and what controls are enabled. It's critical that you define the data model early in the implementation process. You should prepare a data model if you plan to automate processes in the future and therefore expect to perform system integrations. Preparation involves ensuring that your data model matches data fields and IDs with the future integration system. In this way, you ensure that data can be connected.

We recommend that your data model also specifies the auditing requirements, such as what data elements should be tracked, how often data elements should be audited, and who has the authority to make data changes. This information helps your organization ensure a proper audit trail.

## System integrations and reuse

System integration is the process of bringing together separate systems and components into a single, unified system. You should consider it when you're scaling Guides. For example, determine whether it's relevant to link Guides to existing systems, such as a quality management system (QMS) or a learning management system (LMS).

We recommend that you initially handle communication between systems (for example, between Microsoft Power Platform and a QMS) manually. If you identify missing data fields in either system, it's easier to correct this issue manually than by using an automatized process through an integration. In this way, you can detect and correct all minor errors that might occur during implementation before you set up the automated integration.

We recommend that you plan integrations early in the implementation phases. Even though integrations might be developed at a later stage, the work is significantly easier if the data model is prepared in advance.

For scaling over time, automated system integration is recommended. Because it replaces manual controls with automated controls, this type of system integration makes things more robust.

## Notifications

When you create a guide, multiple roles are involved in the different steps of the content life cycle. To ensure that you adhere to validation requirements, and that the process runs smoothly, it's important that the correct roles are notified at the right time. For example, if a guide is awaiting approval in a validation environment, QA should be notified immediately. These notifications can be set up as emails, alerts, or whatever fits your organization's systems. Your organization should ensure that there is a well-functioning flow among the systems and roles that are involved in the content life cycle. Consider taking advantage of existing notification flows that are already working and known by users.

## Next steps

- [Existing Microsoft Power Platform engagement and Guides deployment strategy](strategy-for-existing-power-platform-engagement-and-guides-deployment.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
