---
title: Integration with a quality management system or learning management system strategy
description: Learn about integrating Microsoft Power Platform, a quality management system (QMS), and a learning management system (LMS) with Dynamics 365 Guides in a regulated industry.
ms.date: 03/21/2023
ms.topic: conceptual
author: davepinch
ms.author: davepinch
ms-reviewer: m-hartmann
ms.custom: bap-template
---

# Integration with a quality management system or learning management system strategy

Integrations are useful if you want to automate the manual handover of data between systems such as Microsoft Power Platform and a quality management system (QMS). If you have a well-established approval workflow in your QMS, you can reuse it and its process triggers to automate approval flows.

Integrations allow for automation when:

- QMS record entries are created.
- Guides are made effective in an execution environment.
- Guides are retired so that they are no longer effective (for example, if a standard operating procedure \[SOP\] in the QMS is retired, or the related content is retired).

Regardless of whether integrations are a requirement from the beginning, we recommend that you consider the information in this article during the initial phases of the implementation, because it's also relevant to the user journey and the data model.

## Prerequisites for integration with a QMS and categorization of content in a regulated context

The immersive content that guides consist of is stored in Microsoft Power Platform. This content can't be opened in the QMS itself. Instead, you must create a link between the QMS and the externally stored content (the guide), and associate or create a new document type/record type for digital guides in the QMS. For this document type/record type, define the related requirements and documentation that are needed. A minimum requirement is to have the guide ID from Dynamics 365 Guides and the document/record type ID from the QMS in both systems. These two IDs are recommended parts of the data model from the beginning, even if automatic integration isn't implemented at first. As a prerequisite for enabling automatic integration, the data that will be exchanged must be present in the data model of both systems. 

After the data model is defined, determine what the points of integration are in the user journey, and what activities (actions in the systems) will trigger the data flow between the systems.

There are two ways of doing integrations: process-based integration and technical integration.

## Process-based integration

In this approach, you don't do any technical integration. Instead, you reuse the flow in the QMS and manually transfer data. As was mentioned in [Access control and identity and access management strategy](strategy-for-access-control-and-iam.md), assign a role that is responsible for ensuring the synchronization between the systems when the integration is handled manually.

By manually running integrations, you maintain control of the processes. You can refine those processes without having to adjust the technical integration. We recommend this approach if you're still in the maturing phase and have a limited number of transactions. In this case, thoroughly investigate how the two systems must interact, and prepare the data model in Microsoft Power Platform accordingly. A well-planned data model simplifies technical integration in the future.

## Technical integration

As the solution matures, we recommend that you use technical integration to automate processes that would otherwise be handled manually. There are two options for technical integration: point-to-point integration and API-based middleware integration.

- **Point-to-point integration**: For this option, you connect two apps through custom code. It's a simple and efficient way to connect systems in your business. However, point-to-point integrations aren't designed to keep up with changes. Therefore, the integration falls short whenever changes or updates are introduced into either connected system. In this case, qualify and validate both systems. Because it can be time consuming to keep the integration connectors up to date, this integration option might not be the best choice for you. The frequency of updates to the connected systems affects how viable point-to-point integration is in the long term.

    :::image type="content" source="media/point-to-point-integration.png" alt-text="Diagram that shows an example of point-to-point integration.":::

- **API-based middleware integration**: For this option, software acts as a bridge between two or more systems that must communicate. Middleware integration enables the systems to communicate and establishes data flow among them without requiring that the apps communicate directly. The bridge that the middleware integration creates also separates the system updates. Therefore, both systems don't have to be revalidated if only one of them is changed or updated.

    :::image type="content" source="media/middleware-integration.png" alt-text="Diagram that shows an example of middleware integration.":::

The choice between point-to-point integration and API-based middleware integrations depends on your enterprise architecture strategy and the tools that are available in your organization. If you have middleware integration software, it makes sense to choose the API-based middleware integration. If you don't have middleware integration software, point-to-point integration might be the best fit.

> [!NOTE]
> All technical integrations must be part of the potential Good \{industry\} Practice (GxP) validation and test. This requirement is an argument in favor of starting with process-based integration, because the time to go-live can be reduced. Process-based integration also involves less maintenance work until a critical level of data transfer is needed.

## Integration with an LMS

If you intend to use training material that is developed in Guides, you can connect Guides with your learning management system (LMS). Through this connection, you can transfer users' usage data and information about the completion of guides. The exact setup of this integration depends on the requirements for your specific industry.

The following diagram shows an example of the flow. Training material is stored in Microsoft Power Platform and approved in the QMS. It's then assigned to relevant employees, and execution is documented.

:::image type="content" source="media/integration-pwr-platform-qms-lms.png" alt-text="Diagram that shows an example of an integration between Microsoft Power Platform, a QMS, and an LMS.":::

There are three factors to consider if you plan to connect Guides with your LMS:

- **Integration between the QMS and the LMS**: Establish an integration between the QMS and the LMS to automate the transfer of training from the QMS and the LMS and ensure synchronization. If you don't have an integration, manually ensure that training material is made available from the QMS to the LMS.
- **User-based or device-based licenses**: The way that you use the LMS integration to provide evidence of guide completion depends on whether you have a [user-based or device-based Guides setup](hololens-devices.md#user-based-versus-device-based-setup).

    - If you have a user-based setup, user statistics can provide proof of execution through logs in Microsoft Power Platform. The regulatory requirements that apply to this logging as evidence (for example, GxP and General Data Protection Regulation \[GDPR\]) must be verified with the quality assurance (QA) department in the business and the data protection officer (DPO).
    - If you have a device-based license, user statistics and logs can't be used directly from Microsoft Power Platform. Instead, an app that is developed in Power Apps can be used to create functionality in the training flow that enables employees to provide proof of execution by signing out of their profile. This functionality can be supported by a [digital signature](electronic-records-and-electronic-signature.md) component to make it compliant with regulatory requirements for documentation. Furthermore, you can create integrated functionality that enables users to evaluate the training as additional proof of execution. This approach can also be used for a user-based license if QA or the DPO doesn't accept the Microsoft Power Platform log as evidence of execution.

- **Data model**: As for a QMS integration, we recommend that you prepare your data model for an LMS integration from the very beginning of the implementation. By adding a data field such as **document type** in Microsoft Power Platform, you make integration easier, because that field can be used to identify the records (guides) that must be associated with LMS processes.

## Next steps

- [Electronic records and electronic signatures](electronic-records-and-electronic-signature.md)

[!INCLUDE [footer-include](../../includes/footer-banner.md)]
