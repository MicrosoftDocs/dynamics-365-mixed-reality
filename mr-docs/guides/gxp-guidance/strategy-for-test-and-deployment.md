---
title: Test and deployment strategy
description: Learn about using Power Apps and Microsoft Power Platform for testing and deployment.
ms.date: 03/23/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Test and deployment strategy

We recommend that you develop a governance strategy for testing and deploying the related components of Power Apps and Microsoft Power Platform with links to Azure DevOps and automation. Power Apps is a crucial part of the controls for content and approval that are required in regulated industries to support the rollout of Dynamics 365 Guides.

A governance strategy ensures the basics and best practices for conducting controlled, planned test and deployment activities for Power Apps, facilitated by Azure DevOps, for example. It also helps ensure that you have the required amount of documentation for your regulated industry. Your organization should always confirm what documentation is required. However, a test plan, compliance requirements, version control, and the deployment process are other elements to consider. Sometimes, there are requirements for the user documentation itself.

The purpose of testing and deployment is to keep Microsoft Power Platform environments up to date and handle the apps that support the guide life cycle and approval flows in an Application Lifecycle Management (ALM) approach.

To maintain compliance and ensure that the right quality controls are conducted, it's crucial to keep the apps in the right condition for testing and deployment. One compliance requirement is to ensure that industry requirements have been correctly tracked and managed. Another is to ensure that these industry requirements have been conducted throughout the development process itself. Typically, these compliance requirements are met by defining the software development life cycle and then having it approved by quality assurance (QA). The software development life cycle follows exactly what was defined in your organization when apps were developed on Microsoft Power Platform by using Power Apps. The quality control aspect of it ensures that all relevant standards are verified and met when the apps are developed and tested.

## Software development life cycle

The software development life cycle involves guidance about what must be covered when apps are developed in Power Apps. It can include guidance about which Power App Canvas Templates to follow, which specific themes, fonts, and layouts to use, and which recommended components to use. It also includes guidance about how to conduct QA, risk assessments, testing procedures, and coverage in areas such as unit testing, acceptance testing, security testing, and performance testing. Finally, the software development life cycle includes guidance about how to handle the apps after deployment. It includes details about maintenance requirements and Power Apps processes. It also defines which relevant data must be carried out or, for example, how access to the app should be requested, who should approve it, and when access is reversed.

## ALM

Many of the aspects that are mentioned in this article can serve as a baseline for best practices about the use of ALM. As a starting point, we recommend that you familiarize yourself with what can be achieved by the [environment strategy for ALM](/power-platform/alm/environment-strategy-alm). Use these recommendations together with your organization's requirements to draft the right process for testing and deployment.

## Developing apps to handle the Guides approval flow

To support and handle the Guides process flow, you can incorporate the approval process of your QA organization and combine it with the use of apps that are developed in Power Apps. When these apps are developed for the organization, the existing QA processes must be followed and, to some extent, replicated for them. When you do the test planning of these processes, be in close dialogue with the QA specialists to ensure that each step is conducted in a way that is aligned with the organization. In many cases, the test plan might have to include separate test environments for each part of the process, so that the test doesn't overlap other parts of Microsoft Power Platform. From a compliance perspective, verify that the different components across Microsoft Power Platform still work as expected during a test period. Consider staging a new test environment to allow for parallel verification of the solution and a running environment of Microsoft Power Platform.

## Next steps

- [Segregate guides between organizational entities strategy](strategy-for-segregating-guides-between-organizational-entities.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
