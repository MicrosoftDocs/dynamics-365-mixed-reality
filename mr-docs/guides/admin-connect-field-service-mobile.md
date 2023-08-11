---
title: Set up embedded Guides in Field Service (Dynamics 365) Mobile (preview)
description: Learn about the preview features of embedded guides in the Field Service (Dynamics 365) Mobile app.
ms.author: blairejackiw
author: m-hartmann
ms.date: 08/07/2023
ms.topic: how-to
ms.reviewer: v-wendysmith
ms.custom: bap-template
---

# Set up embedded Guides in Field Service (Dynamics 365) Mobile (preview)

[!INCLUDE [public-preview-banner](../includes/public-preview-banner.md)]

[!INCLUDE [public-preview-note](../includes/public-preview-note.md)]

With embedded Guides (preview), you can create and view Dynamics 365 Guides on your mobile device. The application lets users create and manage interactive instructions that help perform tasks in the real world. You can now use your phone or tablet to create, edit, and view guides.

This feature lets you:

- Access guides using your iOS or Android mobile device (tablet and phone).

- Use guides already created in your existing environment.

- Easily navigate through guide content using sort, filter, and search.

- Access text instruction, photos, videos, Power Apps workflows, and website links.

- Analyze guide execution time from recorded session data that includes location, device type, duration, time spent on each step.

## Limitations

- Embedded guides on mobile devices currently support English only.

## Prerequisites

- An active Dynamics 365 Guides license, either a trial or paid.

- An environment with [Dynamics 365 Guides version 800.6.x installed](/power-platform/admin/manage-apps#install-an-app-in-the-environment-view). To use Guides and Field Service together in the mobile app, ensure both applications are installed on the same environment.

- Field Service (Dynamics 365) Mobile application [installed and updated to the latest version](/dynamics365/field-service/mobile-power-app-overview).

## Set up embedded Guides in Field Service (Dynamics 365) Mobile

1. On your mobile device, open the Field Service app.

1. Sign in using your environment credentials.

1. Enable non-production apps.

1. Select the environment with Guides installed to start the experience. If Field Service is installed on the same environment, [navigate to the the Library option in the bottom navigation](/dynamics365/field-service/access-related-apps-mobile-app) to see your guides.

## Turn on usage data collection for embedded Guides in Field Service (Dynamics 365) Mobile

Dynamics 365 Guides enables customers to capture usage statistics and detailed time-tracking information. This data is turned off by default, but an admin can turn on data collection for specific users.

1. Go to [the Power Apps admin center](https://powerapps.microsoft.com/) and sign in with your admin account.

1. Select **Guides**. A new tab for the Guides model-driven app opens.

1. Change the area to **Settings**.

   :::image type="content" source="media/powerapps-guides-settings.png" alt-text="Screenshot of the Main Settings for Guides in Power Apps.":::  

1. Select **New**.

1. In the **New User Settings** screen, under **User Settings**, enter the following information:

   - **Name**: Opt in for [User name]

   - **Record Guide Usage**: Yes

   - **Belongs To**: [User name]

   :::image type="content" source="media/powerapps-user-settings.png" alt-text="Screenshot of the User Settings for Guides in Power Apps.":::

## Next steps

- [Access related apps form the Field Service (Dynamics 365) Mobile app](/dynamics365/field-service/access-related-apps-mobile-app)
- [Learn about the steps card in Dynamics 365 Guides](operator-step-card-orientation.md)

<!--
# Access Guides from Field Service Mobile app

Set up Guides on mobile to access from Field Service mobile app.

1. Go to [make.powerapps.com](https://make.preview.powerapps.com/) and sign-in.

1. Select the correct environment.

1. Select **Apps**, and then select **Guides**.

1. Select the ellipsis menu (...) and select **Edit**.

1. Select **Settings**.

     ![Selecting the Guides app in Power Apps and select Settings.](media/power-apps-settings.PNG "Selecting the Guides app in Power Apps and then Settings")

1. Expand **Advanced settings** and select **Field Service (Dynamics 365)**.

     ![Selecting Advanced settings and Field Service.](media/settings-advanced-settings.PNG "Selecting Advanced settings and Field Service")

1. Dismiss the Settings popup and select **Save**.

1. Select **Publish**.

## See also

[Create a custom app module based on Field Service Mobile](/dynamics365/field-service/mobile-powerapp-copy-app-module)
-->