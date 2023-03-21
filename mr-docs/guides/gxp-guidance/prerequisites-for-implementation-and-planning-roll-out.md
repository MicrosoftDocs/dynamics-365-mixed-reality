---
title: Prerequisites for implementation and roll-out
description: Learn the prerequisites before implementing Guides in a regulated industry and to help plan the roll-out of the solution
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Prerequisites for implementation and roll-out

As prerequisites for a successful Guides roll-out in regulated industries, it is advised to define the following elements in the initial phases of implementation:

- The Guides user journey
- The data model
- System integrations and reuse
- Notifications

## The Guides user journey

We recommend facilitating a series of internal stakeholder workshops for employees with standard operating procedure (SOP) touchpoints. The group of stakeholders should include, but is not limited to, SOP authors, digital training consultants, business and IT quality assurance (QA) specialists, Power Platform personnel from IT, and operators.

The purpose of the workshops is to receive stakeholder input on the relevant steps and roles involved from the creation of a guide until its archived and identify potential pain points in the life cycle. When this information is mapped in a detailed user journey, it helps you design the right environment structure, the flow of guides between environments, and select the right roles to be associated with each environment. Furthermore, it helps identify existing systems your organization can tap into and processes to reuse or simplify.

## The data model

A data model provides a blueprint for where data comes from, the data format, how it's stored and accessed, and which controls are enabled. It's critical to define the data model early in the implementation process. You should prepare your data model if you wish to automate processes in the future, and therefore expect to make system integrations. You do so by ensuring that your data model matches the data fields and IDs with the future integration system. This ensures that data can be connected.  
  
We also recommend that your data model specifies the auditing requirements such as what data elements to track, how often data elements should be audited, and who has the authority to make data changes. This information helps your organization ensure a proper audit trail.

## System integrations and reuse

System integration is the process of bringing together separate systems and components into a single, unified system. This is relevant to consider when scaling Guides. For instance, determine if it is relevant to link Guides to existing systems such as a Quality Management System (QMS) or a Learning Management System (LMS). Initially, we recommend handling communication between systems, for example, Power Platform and a QMS, manually: If you identify missing data fields within either of the systems, it is easier to correct manually compared to an automatized process through an integration. Hence, you can detect and correct all minor errors that potentially arise during implementation and correct these before setting up the automated integration. We recommend planning integrations early in the implementation phases. Even though integrations might be developed at a later stage, it eases the work significantly if the data model is prepared in advance.

For scaling over time, automated system integration is recommended, as it will also replace manual controls with automated controls, making things more robust.

## Notifications

When creating a guide, there are multiple roles involved in the different steps of the content lifecycle. To ensure that you adhere to validation requirements and that the process runs smoothly, it is important that the correct roles are notified at the right time. For example, if a guide awaits approval in a validation environment, QA should be notified immediately. These notifications can be set up as e-mails, alerts, or whichever fits your organization's systems. Your organization should ensure there is a well-functioning flow among the systems as well as among the roles involved in the content lifecycle. Consider tapping into existing notification flows already working and known by users by system integrations.

Consider the four elements above early in the process as they have significant influence on the overall implementation process and the possibilities for future development.

## Next steps

- [Establishing a Power Platform strategy for regulated industries](strategy-for-existing-power-platform-engagement-and-guides-deployment.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
