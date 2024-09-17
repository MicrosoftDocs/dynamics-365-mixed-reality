---
author: prashantyvr
description: Learn about IP addresses and endpoints required for Dynamics 365 Guides.
ms.author: prashan
ms.date: 04/25/2024
ms.topic: conceptual
title: Network requirements for Dynamics 365 Guides
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Network requirements for Dynamics 365 Guides

Dynamics 365 Guides might require your network admin add the IP addresses and/or endpoints that are required to connect to the Dynamics 365 servers to an approved list. The following list contains the minimum URL endpoints and TCP/UDP ports utilized by Dynamics 365 Guides.

#### Authentication

- login.microsoft.com
- login.microsoftonline.com
- login.live.com
- sts.windows.net
- TCP: 80, 443

#### Teams

- *.skype.com
- *.teams.microsoft.com
- UDP: 3478, 3479, 3480, 3481

If you have specialized needs and/or scale, go to the [Teams comprehensive list](/microsoftteams/prepare-network) for specifics.

#### Microsoft Graph

- graph.microsoft.com
- TCP: 80, 443

#### Dynamics Services

- *.crm.dynamics.com
- *.crm#.dynamics.com (replace # with your region's number). Go to a [full list of datacenter regions](/power-platform/admin/new-datacenter-regions).
- TCP: 80, 443

#### Sharepoint/OneDrive

- *.sharepoint.com
- TCP: 80, 443

#### Power Apps

- service.powerapps.com
- api.bap.microsoft.com
- TCP: 80, 443

#### Documentation 

- aka.ms
- powerbi.microsoft.com
- go.microsoft.com
- privacy.microsoft.com
- www.microsoft.com 
- TCP: 80, 443

#### Windows Notification Service

Go to [Enterprise Firewall Configurations to Support WNS Traffic](/windows/apps/design/shell/tiles-and-notifications/firewall-allowlist-config).

## See also

- [Power Platform URLs and IP address ranges](/power-platform/admin/online-requirements#ip-addresses-and-urls)
- [Deployment Playbook](admin-deployment-playbook.md)
- [Other HoloLens endpoints](/hololens/hololens-offline)
