---
title: Purpose of validation and traceability
description: Learn about the reasons for validation and traceability in a regulated industry 
ms.date: 03/09/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
---

# Purpose of validation and traceability

The purpose of validation is to ensure the consistency of any process or system, and to make sure it is documented. Having the system validated is a requirement from regulating agencies such as the US Food and Drug Administration (FDA) (specifically for Life Science organizations). Validation is defined as follows: 

"*Validation means confirmation by examination and provision of objective evidence that the particular requirements for a specific intended use can be consistently fulfilled* ([<u>FDA</u>](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/cfrsearch.cfm?fr=820.3)) 

"*Establishment of documentary evidence that provides a high degree of assurance that a planned process will be uniformly in accordance with the expected specified results.*" ([<u>WHO</u>](https://www.who.int/teams/health-product-and-policy-standards/standards-and-specifications/norms-and-standards-for-pharmaceuticals/guidelines/production) guidance on the requirements of good manufacturing practices (GMP)) 

  

The above definitions have the following elements in common, in accordance with expected results:  

-   Generate evidence 

-   Compliance with regulations 

-   Fulfill requirements 

  

Validation of computerized systems is a documented process to ensure that the system does exactly what it was designed to do in a consistent and reproducible way. Validation ensures the integrity and security of data processing, product quality, and compliance with regulations that apply to GxP.  
 

How to validate a computerized system is described in Standard Operation Procedures (SOP) and guidelines which are created and defined by the life science organization. For implementation of the validation process of computer systems, it is useful to view it as **a project**. (GAMP 5)

When starting the project, the high-level plan for the new solution should be in place, and then start the implementation project with the following phases:  
 

- **Planning**: In this phase, the requirements and specifications should be clear enough for an initial risk assessment and ultimately for a correct definition of verification tests (protocols). During this phase, you deliver the validation plan document which defines the entire validation strategy and deliverables. The strategy should be in accordance with the quality management system and policies. 

- **Specification, configuration, and coding**: In this phase, all design specifications are made with the level of detail required by the type of system and its use. Developers need to choose and use the development methods and models most appropriate to the coding and configuration requirements and based on the approved specifications. All these activities are done in the development environment. In this phase, testing is more focused on verification of the units/features from a developer point of view. An example of such tests are unit testing, statistic testing of code, and integration testing. Those testing activities could be automated by tools. 

- **Testing**: This phase confirms that the specifications have been met through inspections and testing of the system. The test activities are done in a prepared and suitable TEST environment. The test environment needs to resemble the production environment to ensure that conditions are the same, and to make sure you don't need to repeat tests in the production environment. The scope of the test effort should be driven by the risk. Risk analysis can help you understand potential hazards which can have an impact on the product quality, patient safety, or data integrity.. Those potential hazards must be mitigated by having controls in place and proof of testing. If there is a high risk somewhere, you need to have appropriate test scenarios to prove that the solution design is without potential failure. 

- **Reporting and release**: In this phase, the system must be acceptable for use in the production environment according to a documented and controlled process. A system validation completion must be prepared at project closure, summarizing the activities undertaken and any deviations there might be from the validation plan. The validation of the system should be completed prior to release for use. 

A good overall way of illustrating the project phases is the following V-model supported by <u>[GAMP 5](https://ispe.org/publications/guidance-documents/gamp-5-guide-2nd-edition) 2nd edition</u>: A Risk-Based Approach to Compliant GxP Computerized Systems.

![](media/image16.png)

The V-model can be viewed not only as the development activities and testing of the system, but also their sequence, their interrelationships, and the validation process of the deliverables applicable to the validated computerized system. You need to keep and maintain interrelationships between requirements, specifications, and tests. This interrelationship is documented in the Traceability Matrix used within regulated areas.  
   

The Traceability Matrix ensures that: 

-   Requirements are fulfilled by the solution design. This means that each requirement is traced to the functions, controls, configurations, or design elements<u>.</u> 

-   Requirements are tested or verified. This demonstrates the solution design fulfills requirements, as appropriate. 

  

The Traceability Matrix document has its own specific benefits: 

-   Supports the design review 

-   Helps define the scope of the regression testing 

-   Provides support during inspection or audit activities 

-   Provides support for potential changes

## Platform qualification

Regulated industries need to qualify the Microsoft Power Platform as infrastructure before implementing Guides. To do so, the following tasks are required as a minimum:

-   Initial Risk Assessment (asses GxP applicability)

-   Vendor Assessment (audit of vendor – can be virtual/physical/postal)

-   Qualification Plan

-   Platform Design Technical Specification

-   Risk Assessment (e.g., the risk of having the wrong version of a guide made available to operators)

-   Testing

    -   Installation testing e.g., testing that the environments are correctly installed

    -   Operational testing e.g., testing that the right users have the right accesses

-   Summary Qualification Report

-   Platform/Operational Manual, Training Material

## Application validations

Applications (such as Guides and Power Apps) that supports business processes within regulated industries must be validated, which means that your organization needs to complete the following tasks:

-   Initial Risk Assessment

-   Validation Plan

-   User Requirements

-   Risk Assessment

-   Application Functional/Configuration Technical Specification

-   Testing (IQ/OQ/UAT)

    -   Operational testing e.g., verifying a function

    -   User Acceptance Test

-   Traceability Matrix

-   Summary Validation Report

-   Application/Operational Manual, Training Material


