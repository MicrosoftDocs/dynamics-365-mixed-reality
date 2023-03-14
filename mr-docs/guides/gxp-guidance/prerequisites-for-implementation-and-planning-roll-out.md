---
title: Prerequisites for implementation and planning roll-out
description: Learn the prerequisites before implementing Guides in a regulated industry and to help plan the roll-out of the solution
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Prerequisites for implementation and planning roll-out

As prerequisites for a successful Guides roll-out in regulated industries, it is advised to define the following elements in the initial phases of implementation:

- The Guides user journey
- The data model
- System integrations and reuse
- Notifications

**The Guides user journey**

It is recommended to facilitate a series of internal stakeholder workshops for employees with Standard Operation Procedure (SOP) touchpoints. The group of stakeholders should include, but is not limited to, SOP authors, digital training consultants, business and IT QAs, Power Platform personnel from IT, and operators.

The purpose of the workshops is to receive stakeholder input on the relevant steps and roles involved from the creation of a guide until its archiving and identify potential pain points in the life cycle. When this information is mapped in a detailed user journey, it will help you design the right environment structure, the flow of guides between environments, and select the right roles to be associated with each environment. Furthermore, it will help identify existing systems your organization can tap into and processes to reuse and/or simplify.

**The data model**

A data model provides a blueprint for where data comes from, the data format, how it is stored, accessed and which controls are enabled. It is critical to define the data model early in the implementation process: If you wish to automate processes in the future, and therefore expect to make system integrations, you should prepare your data model for this. You do so by ensuring that your data model matches the data fields and IDs with the future integration system. This ensures that data can be connected.  
  
It is also recommended that your data model specifies the auditing requirements such as what data elements needs to be tracked, how often data elements need to be audited, and who has the authority to make data changes. This will help your organization to ensure a proper audit trail.

**System integrations and reuse**

System integration is the process of bringing together separate systems and components into a single, unified system. This is also relevant to consider when scaling Guides. For instance, determine if it is relevant to link Guides to existing systems such as a Quality Management System (QMS) or a Learning Management System (LMS). However, initially, it is recommended to handle communication between systems, for example, the Power Platform and a QMS, manually: If you identify missing data fields within either of the systems, it is easier to correct manually compared to an automatized process via an integration. Hence, you can detect and correct all minor errors that potentially arises during implementation and correct these before setting up the automated integration. It is, however, recommended to plan integrations early in the implementation phases. Even though integrations might be developed at a later stage, it eases the work significantly if the data model is prepared in advance.

For scaling over time, automated system integration is a recommendation, it will also replace manual controls with automated controls, making things more robust.

**Notifications**

When creating a guide, there are multiple roles involved in the different steps of the content lifecycle. To ensure that you adhere to validation requirements, and that the process runs smoothly, it is important that the correct roles are notified at the right time. For example, if a guide awaits approval in an environment for validation, QA needs to be notified immediately. These notifications can be set up as e-mails, alerts, or whichever fits your organization's systems. Your organization will want to ensure there is a well-functioning flow amongst the systems as well as amongst the roles involved in the content lifecycle. It might be of value to consider tapping into existing notification flows already working and known by users by system integrations.

The four elements above need to be considered early in the process as they have significant influence on the overall implementation process and the possibilities for future development.

## Next steps

- [Establishing a Power Platform strategy for regulated industries](strategy-for-existing-power-platform-engagement-and-guides-deployment.md)
