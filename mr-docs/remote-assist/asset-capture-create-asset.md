---
title: Create a new asset record
author: bencorn
description: Learn how to create new asset records in Remote Assist.
ms.author: becorn
ms.date: 5/31/2020
ms.service: crm-online
ms.topic: article
ms.reviewer: krbjoran
---
# Create asset records

Assets let you track the equipment you operate, inspect, maintain, and repair. They provide a simple and organized way to keep track of data generated in the field through Remote Assist, like photos with spatial annotations taken during an inspection and text notes entered after service is performed. Overtime, an asset record serves as a visual historical record and audit trail of how an asset changed over time and the various work performed on the asset.

In this article, you will learn how to create new asset records, import  assets records from another system, and view the asset records in the Remote Assist web app.

## Prerequisites

To complete this article, you need:

- **Access to the environment Remote Assist is installed in**. You will be accessing the Remote Assist app to create a new record.
- (Optional) **Access to the system where your asset data is currently stored**, this could be a database, Excel spreadsheet, or some other software.

## Create assets

Assets can be created:

1. Manually through the Remote Assist app
2. Imported
3. Through a Power Platform data integration project

### Manually create customer assets

From the main menu of your environment, select **Remote Assist** > **Assets** > **+ New**

![Screenshot of the Remote Assist web app.](./media/AC_CreateAsset.png "Remote Assist app")

For the following fields:

- **Name**: Enter a reference name or title for the asset. This can be the make and model of the asset, the name of the product in the product catalog, a general name like "HVAC Unit," or even hold descriptive information like "HVAC Unit 2nd Floor".
- **Category**: Add or create an asset category that serves as a label to organize assets into useful groups by function, model, and so on, based on your business needs.
- **Service Account**: If you maintain the asset on behalf of a customer, choose an account from the lookup to represent the location and customer of the asset.
- **Product**: Add the product that the asset correlates to. An example would be the make and model of a specific generator you maintain and operate.
- **Parent Asset**: Remote Assist supports hierarchical asset structures. For example, a part can be the child of a widget, which is the child of a machine. You can have as many parent-child relationships as needed. Use this field to identify the direct parent of this asset. The Master Asset shows the top-level parent in the relationship automatically. Additionally, you can use the Sub Asset grid on the form to add child  assets.

When done, click **Save**.

## Import assets

There are two ways to integrate your existing asset catalog for use in Remote Assist and in other Dynamics 365 applications.

1. Export your existing asset data to a CSV or Excel sheet and import the data to Common Data Service for use in Remote Assist.
2. Setup a **Data integration project** to enable the flow of data between Remote Assist and your external data source (automatically updates asset data).

This tutorial will go through the steps for option 1. If you want to learn more about data integration projects, please refer to the docs here: [Integrate data into Common Data Service
](https://docs.microsoft.com/power-platform/admin/data-integrator)

### Download the template

1. Sign in to the [Power Platform Admin Center](https://admin.powerplatform.com) as an admin (Dynamics 365 service admin, Global admin, or Power Platform service admin).
2. Select **Environments**, find the environment Remote Assist is installed in, and select the dots for **More environment actions**.
3. Select **Settings**, then select **Templates** > **Data import templates**.
4. From the dropdown, select the **Customer Asset** record type.
5. Select **Download**.

### Import data to Common Data Service

In the downloaded template file, you will find a set of fields. The only required field is the **Name** field. This is the name of the asset, such as "Fabrikam Generator - 0039 - 4th Floor NW" and is the primary way you will search and identify asset records. Other optional fields include Account, Product, and Category. To use these fields in the template, the data must already exist in Common Data Service. For example, if you import an asset record with a category called "Pump", the "Pump" category record must already exist, otherwise the record will fail to import.

For the purposes of this tutorial, we will leave these blank and only use the asset name field. You can always go back and add or import the data later. To learn more about importing data to Dynamics 365, see [Import data](https://docs.microsoft.com/powerapps/developer/common-data-service/import-data).

1. Open the downloaded Excel (.xlsx) file.
2. Insert your existing asset record data into the sheet and save the file.
3. From the main menu of your environment, select **Remote Assist** > **Assets** > **Import from Excel**.
4. Select the template file and then select **Next**.
5. Select **Finish Import**. Depending on the number of records you are importing, this process may take a while. Periodically refresh the page to see your records start to populate the asset list.

## Next steps

In this tutorial, you learned how to create asset records and import an existing asset catalog to Common Data Service. To learn how to view these assets in Remote Assist on HoloLens 2 and capture asset data with spatial markup, see:

> [!div class="nextstepaction"]
> [Capture asset data in HoloLens](./asset-capture-create-asset.md)