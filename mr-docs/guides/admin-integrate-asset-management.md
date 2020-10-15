---
author: Mamaylya
description: Learn how to integrate Dynamics 365 Supply Chain Management with Dynamics 365 Guides to take advantage of mixed-reality guides in day-to-day service and maintenance workflows.
ms.author: mamaylya
ms.date: 10/15/2020
ms.service: crm-online
ms.topic: article
title: Integrate Dynamics 365 Supply Chain Management with Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Integrate Dynamics 365 Supply Chain Management with Dynamics 365 Guides

You can integrate Microsoft Dynamics 365 Supply Chain Management with Dynamics 365 Guides in two ways:

- Through production processes

- Through asset management

## Production processes

You can integrate production processes from Supply Chain Management so first-line workers can benefit from mixed-reality guides in various areas of their work, including: assembly, service, operations, certification, and safety.

You can attach guides to various aspects of production control, including:

- [Resources](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#resources)

- [Resource groups](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#resource-groups)

- [Released products](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#released-products)

- [Formulas](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#formulas)

- [Formula versions](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#formula-versions)

- [Bills of material (BOMs)](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#bom)

- [BOM versions](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#bom-versions)

- [Routes](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#routes)

- [Route versions](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#route-versions)

- [Route operation relations](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#route-operation-relations)

When a first-line worker chooses a job on the shop floor through Supply Chain Management, the worker can see [the relevant guides](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#logic) on the job card. When the worker chooses a specific guide, a QR code for that guide is shown on the screen. The worker then uses their HoloLens to scan the QR code, which launches Dynamics 365 Guides and shows the required instructions. 

![Screen shot of QR code used to open a guide from Dynamics 365 Supply Chain Management](media/scm-integration-qr-code-scan.PNG "Screen shot of QR code used to open a guide from Dynamics 365 Supply Chain Management")
 
[Learn more about integrating Dynamics 365 Guides with various aspects of production control](https://docs.microsoft.com/dynamics365/supply-chain/production-control/instruction-guides-in-production-overview#logic)

## Asset management

You can integrate the **Asset Management** module in Supply Chain Management with Dynamics 365 Guides to take advantage of mixed-reality guides in your day-to-day service and maintenance workflows. If a guide is associated with an Asset Management work order, when a worker opens the work order's Maintenance Checklist in the Finance and Operations (Dynamics 365) mobile app (1), the line details show that a guide is available (2). The worker can then find and open the guide in the Dynamics 365 Guides HoloLens app (3).

![Integrated Asset Management guide](media/asset-management-integration.JPG "Integrated Asset Management guide")

[Learn more about integrating Asset Management with Dynamics 365 Guides](https://docs.microsoft.com/dynamics365/supply-chain/asset-management/asset-management-guides-integration)

## See also

[Integrate Dynamics 365 Field Service with Dynamics 365 Guides](field-service.md)
