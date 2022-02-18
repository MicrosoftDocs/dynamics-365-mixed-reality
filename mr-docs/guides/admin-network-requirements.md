

# Network requirements for Dynamics 365 Guides

The following list contains the minimum URL endpoints and TCP/UDP ports utilized by Dynamics 365 Guides.

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
