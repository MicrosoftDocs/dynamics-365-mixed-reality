---
author: Mamaylya
description: Learn about IP addresses and endpoints required for Dynamics 365 Guides 
ms.author: mamaylya
ms.date: 02/18/2022
ms.topic: article
title: Network requirements for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Network requirements for Dynamics 365 Guides

Dynamics 365 Guides is a cloud-based application and might require that your network admin add, to an approved list, the IP addresses and/or endpoints that are required to connect to the Dynamics 365 servers. The following list contains the minimum URL endpoints and TCP/UDP ports utilized by Dynamics 365 Guides.

#### Authentication
- login.microsoft.com
- login.microsoftonline.com
- login.live.com
- sts.windows.net
- TCP: 80, 443

#### Teams

- *.registrar.skype.com
- *.teams.microsoft.com
- UDP: 3478, 3479, 3480, 3481

If you have specialized needs and/or scale, see the [Teams comprehensive list](/microsoftteams/prepare-network) for specifics.

#### Microsoft Graph
- graph.microsoft.com
- TCP: 80, 443

#### Dynamics Services
- *.crm.dynamics.com
- *.crm#.dynamics.com (replace # with your region's number). See a [full list of datacenter regions](https://docs.microsoft.com/power-platform/admin/new-datacenter-regions).
- TCP: 80, 443

#### Sharepoint/OneDrive
- *.sharepoint.com
- TCP: 80, 443

#### Power Apps
- service.powerapps.com
- TCP: 80, 443

#### Documentation 
- aka.ms
- powerbi.microsoft.com
- go.microsoft.com
- privacy.microsoft.com
- www.microsoft.com 
- TCP: 80, 443

#### Windows Notification Service

See [Enterprise Firewall Configurations to Support WNS Traffic](https://docs.microsoft.com/windows/apps/design/shell/tiles-and-notifications/firewall-allowlist-config)

## See also

- [Unblocking IP addresses and URLs](/power-platform/admin/online-requirements#ip-addresses-and-urls)
- [Deployment Playbook](admin-deployment-playbook.md)
