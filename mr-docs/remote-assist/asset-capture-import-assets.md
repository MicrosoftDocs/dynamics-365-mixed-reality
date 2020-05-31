---
title: Import an existing asset catalog
author: bencorn
description: Learn how to import existing asset records to Common Data Service for use in Remote Assist.
ms.author: becorn
ms.date: 5/31/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Import an existing asset catalog

Learn how to import an existing asset catalog data into Common Data Service for use in Remote Assist.

In this tutorial, you will download the import template, learn how to populate data, run the import wizard, and view the imported data in the Remote Assist web app.

## Prerequisites

To complete this article, you need:

- **Access to the environment Remote Assist is installed in**. You will be accessing the Remote Assist app to import asset data.
- **Access to the system where your asset data is currently stored**, this could be a database, Excel spreadsheet, or some other software.

## Select an import method

There are two ways to integrate your existing asset catalog for use in Remote Assist and in other Dynamics 365 applications.

1. Export your existing asset data to a CSV or Excel sheet and import the data to Common Data Service for use in Remote Assist.
2. Setup a **Data integration project** to enable the flow of data between Remote Assist and your external data source (automatically updates asset data).

This tutorial will go through the steps for option 1. If you want to learn more about data integration projects, please refer to the docs here: [Integrate data into Common Data Service
](https://docs.microsoft.com/power-platform/admin/data-integrator)

## Download the template

1. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. Select **Environments**, find the environment Remote Assist is installed in, and select the dots for **More environment actions**.
3. Select **Settings**, then select **Templates** > **Data import templates**.
4. From the dropdown, select the **Customer Asset** record type.
5. Select **Download**.

## Import data to Common Data Service

In the downloaded template file, you will find a set of fields. The only required field is the **Name** field. This is the name of the asset, such as "Fabrikam Generator - 0039 - 4th Floor NW" and is the primary way you will search and identify your asset records. Other optional fields include Account, Product, and Category. To use these fields in the template, the data must already exist in Common Data Service. For example, if you import an asset record with a category called "Pump", the "Pump" category record must already exist, otherwise the record will fail to import.

For the purposes of this tutorial, we will leave these blank and only use the asset name field. You can always go back and add or import the data later. To learn more about importing data to Dynamics 365, see [Import data](https://docs.microsoft.com/powerapps/developer/common-data-service/import-data).

1. Open the downloaded Excel (.xlsx) file.
2. Insert your existing asset record data into the sheet and save the file.
3. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
4. Select **Environments**, find the environment Remote Assist is installed in, and select the dots for **More environment actions**.
5. Select **Open environment**, then select the **Remote Assist** app once the environment has loaded.
6. From the top toolbar of the Remote Assist app, select **Import from Excel**.
7. Select the template file and then select **Next**.
8. Select **Finish Import**. Depending on the number of records you are importing, this process may take a while. Periodically refresh the page to see your records start to populate the asset list.

## Next steps

In this tutorial, you learned how to do this...

> [!div class="nextstepaction"]
> [Create assets](./asset-capture-create-asset.md)