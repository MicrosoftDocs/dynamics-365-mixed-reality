---
title: Test and deployment strategy
description: Learn about using Power Apps and Power Platform for test and deployment
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Test and deployment strategy

We recommend developing a governance strategy around the test and deployment of Power Apps as well as Power Platform's related components with links to DevOps and automation. Power Apps is a crucial part of the controls of content and approval required within a regulated industry to support the roll-out of Guides.  
  
A governance strategy ensures the basics and best practices of conducting controlled, planned, test and deployment activities for Power Apps facilitated by, for example, Azure DevOps. It also helps secure the required amount of documentation for your regulated industry. Your organization should always confirm what documentation is required. However, a test plan, compliance requirements, version control, and deployment process are elements to consider. Sometimes, there are requirements for the user documentation itself.

The purpose of test and deployment is to keep Power Platform environments up-to-date, and to handle the Power Apps that support the guides lifecycle and approval flows from an Application Lifecycle Management (ALM) approach.

Keeping the Power Apps in the right condition for test and deployment is crucial for maintaining compliance and for ensuring that the right quality controls are conducted. One compliance requirement is to ensure that industry requirements have been tracked and managed properly. Another compliance requirement is to ensure that these industry requirements have been conducted throughout the development process itself. Typically, this is done by defining the software development life cycle (SDLC), and subsequently having it approved by quality assurance (QA). This SDLC follows exactly what has been defined in your organization when developing Power Apps on Power Platform. The quality control aspect of it is to ensure that all relevant standards have been verified and met when developing and testing the Power Apps.

## Software development lifecycle

The SDLC entails guidance for what needs to be covered when developing Power Apps. It can include guidance for which Power App Canvas Templates to follow, specific themes, fonts, and layouts, as well as which recommended components to use. An SDLC also covers areas on how to conduct quality assurance, risk assessment, testing procedures, and coverage within areas like unit testing, acceptance testing, security testing, and performance testing. Lastly, the SDLC defines how to handle the Power App after deployment. It includes details on maintenance requirements, Power App processes, which relevant data that needs to be carried out, or, for example, how access to the app should be requested, who should approve it, and when access is reverted again.

## Application lifecycle management

Many of the aspects mentioned in this section can be used as a baseline for best practices on the usage of ALM. As a starting point, we recommend familiarizing yourself with what can be achieved by the [environment strategy for ALM](/power-platform/alm/environment-strategy-alm). Use these recommendations combined with your organization's requirements to draft the right process around test and deployment.

## Developing Power Apps for handling Guides approval flow

The support and handling of the Guides process flow can be achieved by incorporating the approval process of your QA organization and combining this with the utilization of Power Apps. When developing these Power Apps for the organization, it needs to follow, and to some extend replicate, the existing QA processes into the Power Apps. When you are conducting the test planning of these processes, be in close dialogue with the QA specialists to ensure that each step is conducted in alignment with the organization. In many cases, this might mean the test plan includes separate test environment(s) for each part of the process, so the test is not overlapping with other parts of Power Platform. From a compliance perspective, verify that the different components across Power Platform are still operating as expected during a test period. Consider staging a new test environment to allow parallel verification of the solution and a running Power Platform.

## Next steps

- [Strategy for segregating guides between organizational entities](strategy-for-segregating-guides-between-organizational-entities.md)
