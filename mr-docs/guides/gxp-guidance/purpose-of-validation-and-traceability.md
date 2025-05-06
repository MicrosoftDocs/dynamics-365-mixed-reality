---
title: Purpose of validation and traceability
description: Learn about the reasons for validation and traceability in a regulated industry.
ms.date: 03/21/2023
ms.topic: article
author: prashantyvr
ms.author: prashan
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Purpose of validation and traceability

The purpose of validation is to ensure that a process or system is consistent and documented. System validation is a requirement of regulating agencies. For life science organizations, for example, the regulating agencies include the United States Food and Drug Administration (FDA).

[FDA](https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfcfr/cfrsearch.cfm?fr=820.3) defines *validation* as follows:

> Confirmation by examination and provision of objective evidence that the particular requirements for a specific intended use can be consistently fulfilled.

[The World Health Organization (WHO)](https://www.who.int/teams/health-product-and-policy-standards/standards-and-specifications/norms-and-standards-for-pharmaceuticals/guidelines/production) defines *validation* as follows in its guidance about the requirements for good manufacturing practices (GMP):

> Establishment of documentary evidence that provides a high degree of assurance that a planned process will be uniformly in accordance with the expected specified results.

These definitions have the following elements in common, in accordance with expected results:  

- Generation of evidence
- Compliance with regulations
- Fulfillment of requirements

Validation of computerized systems is a documented process for ensuring that the system does exactly what it was designed to do in a consistent and reproducible way. Validation ensures the integrity and security of data processing, product quality, and compliance with regulations that apply to Good \{industry\} Practice (GxP).

The process for validating a computerized system is described in standard operating procedures (SOP) and guidelines that are created and defined by the regulated industry, such as life science organizations. For the validation of computerized systems, it's useful to view implementation of the process as a **project**, as described in the International Society for Pharmaceutical Engineering's (ISPE's) *Good Automated Manufacturing Practice (GAMP) 5: A Risk-Based Approach to Compliant GxP Computerized Systems*.

Before you start the implementation project, a high-level plan for the new solution should be in place. Then start the project by completing the following phases:

- **Planning**: In this phase, the requirements and specifications should be clear enough for an initial risk assessment and, ultimately, for a correct definition of verification tests (protocols). During this phase, you deliver the validation plan document that defines the whole validation strategy and all the deliverables. The strategy should be in accordance with the quality management system (QMS) and policies.
- **Specification, configuration, and coding**: During this phase, all design specifications are made at the level of detail that is required by the type of system and its use. Developers choose and use the development methods and objects that are most appropriate to the coding and configuration requirements and based on the approved specifications. All these activities are done in the development environment. During this phase, testing is more focused on verification of the units or features from a developer perspective. Examples of the testing activities include unit testing, statistic testing of code, and integration testing. Tools can automate these testing activities.
- **Testing**: This phase confirms that the specifications have been met through inspections and testing of the system. The testing activities are done in a prepared and suitable test environment. The test environment must resemble the production environment to ensure that conditions are the same and that you don't have to repeat tests in the production environment. The risk should drive the scope of the test effort. Risk analysis can help you understand potential hazards that can have an impact on product quality, patient safety, or data integrity. Those potential hazards must be mitigated through controls that are in place and proof of testing. If there is a high risk somewhere, have appropriate test scenarios to prove that the solution design is without potential failure.
- **Reporting and release**: In this phase, the system must be acceptable for use in the production environment according to a documented and controlled process. At project closure, a system validation completion must be prepared to summarize the activities that were undertaken and any deviations from the validation plan. The validation of the system should be completed before the system is released for use.

The following illustration shows the V-model that is supported by [GAMP 5, 2nd edition](https://ispe.org/publications/guidance-documents/gamp-5-guide-2nd-edition). It provides a good overall way of viewing the project phases.

:::image type="content" source="media/vmodel-gamp5.png" alt-text="Diagram that shows an example of project phases that use the V-model supported by GAMP 5 2nd edition.":::

The V-model can be viewed not only as the development activities and testing of the system, but also their sequence, their interrelationships, and the validation process of the deliverables that are applicable to the validated computerized system. You must keep and maintain interrelationships between requirements, specifications, and tests. This interrelationship is documented in the Traceability Matrix that is used in regulated areas.

The Traceability Matrix ensures that:

- Requirements are fulfilled by the solution design. In other words, each requirement is traced to the functions, controls, configurations, or design elements.
- Requirements are tested or verified to demonstrate that the solution design fulfills requirements, as appropriate.

The Traceability Matrix has the following benefits:

- It supports the design review.
- It helps define the scope of the regression testing.
- It provides support during inspection or audit activities.
- It provides support for potential changes.

## Platform qualification

Regulated industries must qualify the Microsoft Power Platform as infrastructure before they implement Guides. Platform qualification requires the following tasks at a minimum:

- Initial risk assessment (assessment of GxP applicability)
- Vendor assessment (audit of a vendor, whether virtual, physical, or postal)
- Qualification plan
- Platform design technical specification
- Risk assessment (for example, assessment of the risk of making the wrong version of a guide available to operators)
- Testing:

    - Installation testing (for example, testing that the environments are correctly installed)
    - Operational testing (for example, testing that the right users have the right accesses)

- Summary qualification report
- Platform or operational manual, and training materials

## Application validations

Applications (such as Guides and Power Apps) that support business processes in regulated industries must be validated. Therefore, your organization must complete the following tasks:

- Initial risk assessment
- Validation plan
- User requirements
- Risk assessment
- Application functional specification or configuration technical specification
- Testing (installation qualification \[IQ\], operational qualification \[OQ\], and user acceptance testing \[UAT\]):

    - Operational testing (for example, verifying a function)
    - UAT

- Traceability Matrix
- Summary validation report
- Application or operational manual, and training materials

## Next steps

- [Maintenance of the qualified and validated status](maintenance-of-the-qualified-and-validated-status.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
