---
author: Mamaylya
description: This topic explains how to add a tab on HoloLens that shows a custom list of guides for a specific set of users.
ms.author: mamaylya
ms.date: 09/02/2020
ms.service: crm-online
ms.topic: article
title: Show a list of guides on a custom tab for a specific set of Dynamics 365 Guides users
ms.reviewer: v-brycho
---

# Show a list of guides on a custom tab for a specific set of Dynamics 365 Guides users

If you want to create a custom list of guides for a specific user or set of users in Microsoft Dynamics 365 Guides, you can create a custom view. Operators access the view through a custom tab on HoloLens. This tab contains only the guides that are defined by the custom view. 

The following illustration shows an example of a custom tab that contains a custom list of guides.

![Example of a custom view that appears on a HoloLens tab](media/custom-view-hololens-tab.PNG "Example of a custom view that appears on a HoloLens tab")

Custom views are useful when you want to show a set of guides that is related to a specific workflow. For example, you might want to show a different set of guides to each team or business unit. Alternatively, you might want to show a list of guides that is targeted at a specific type of operator role.

## Prerequisites

To create a custom view, you must have the following prerequisites:

- Dynamics 365 Guides solution version 104.1907.0.33 or later

- Dynamics 365 Guides PC and HoloLens app versions 104.1907.19001 or later

You must also have the **System Administrator** role for the Dynamics 365 Guides instance that you're working with. Additionally, it's useful to have a general understanding of [Common Data Service](https://docs.microsoft.com/powerapps/maker/common-data-service/data-platform-intro), the database that Dynamics 365 Guides is based on.

## Overview of creating a custom view

The process of creating a custom view involves these basic steps:

1. Create a new entity in Common Data Service. This entity contains the fields that will be included in the view. (It must contain at least two fields.)

2. Create the view.

3. Create a Guides view configuration record.

4. Use the App Designer to add specific guides to the list that is shown in the view.

The remaining sections of this topic describe each step in detail.

## Step 1: Create a new entity in Common Data Service

> [!NOTE]
> If you want to use an existing entity instead of creating a new entity, skip ahead to the [Step 2: Create the view](#step-2-create-the-view) section.

1. Go to [https://powerapps.microsoft.com](https://powerapps.microsoft.com) and sign in as an admin.

    ![powerapps.microsoft.com](media/custom-view-powerapps.PNG "powerapps.microsoft.com")
    
2. In the **Environments** pane on the right side of the screen, select the instance where the Dynamics 365 Guides solution is installed (the instance you want to add the custom tab to).

    ![Environments pane showing instances](media/custom-view-select-instance1.PNG "Environments pane showing instances")

2. In the left pane, select **Data**, and then select **Entities**. Then select **New entity**.

    ![Create an entity](media/custom-view-new-entity.PNG "Create an entity")

3. In the **New entity** dialog box, enter a display name (for example, **Custom Tab**).

    ![Enter a display name](media/custom-view-entity-display-name.PNG "Enter a display name")

    > [!IMPORTANT]
    > The display name must be singular. If it's plural, the tab won't appear correctly on HoloLens.

4. Select **Create**.

5. While the new entity is open, select **Add field**.

6. In the **Field properties** dialog box, follow these steps:

    1. In the **Display name** field, enter **Date and Time**.

    2. In the **Data type** field, select **Date and Time**.

        ![Enter Date and Time field properties](media/custom-view-date-time-field.PNG "Enter Date and Time field properties")

    3. Select **Done**.

7. Select **Add field** again, and then, follow these steps in the **Field properties** dialog box:

    1. In the **Display name** field, enter **Guide**.

    2. In the **Data type** field, select **Lookup**. You will use this field to search the database and assign a guide to the entity through the view.

    3. In the **Related entity** field, enter **Guide**.

        ![Enter Guide field properties](media/custom-view-lookup-field.PNG "Enter Guide field properties")

    4. Select **Done**.

8. In the lower-right corner of the page, select **Save Entity**.

## Step 2: Create the view

In this step, you will add a view to the entity that you created in the previous section. This view will include the same fields that you added to the new entity.

The following rules apply to the view:

- It must have at least two columns. Additional columns are optional. The example that follows includes a third column.

- The first column must be a **Date and Time** field (that is, it must have the **Date and Time** data type), and the field can't be empty.

- The second column must be a lookup to the **msmrw\_guide** entity, and the field can't be empty.

- If a formatted value is available, it will be used.

- Nonempty values are concatenated and shown below the guide name.

The following illustration shows an example of a tab that is named **Custom Tab** on HoloLens. It also shows where the values for each part of the tab come from.

![HoloLens tab](media/custom-view-hololens-tab-sources.PNG "HoloLens tab")

1. The name of the view that you create

2. The **Guides** field

3. The **Date and Time** field

4. An additional field (This field can be any field that you want to add.)

### Create the view

1. Make sure that the entity that you created in the previous section is open.

    > [!NOTE]
    > You can't create the view on the **msmrw\_guide** entity.

2. Select **Views**, and then select **Add view**.

    ![Add a view](media/custom-view-create-view.PNG "Add a view")

3. In the **Create a view** dialog box, enter a name for the view. This name will be shown on the HoloLens tab.

    ![Enter a view name](media/custom-view-view-name.PNG "Enter a view name")

4. Select **Create**.

5. Select **Add column**, and then select **Date and Time**.

    ![Add a column](media/custom-view-add-columns.PNG "Add a column")

6. Select **Add column** again, and then select **Guide**.

    ![Add another column](media/custom-view-columns-added.PNG "Add another column")

    > [!NOTE]
    > You can drag columns to move them after they are created.

7. In the upper-right corner of the page, select **Save**, select **Publish**, and then refresh the page.

8. Copy and save the record ID for the saved query. This record ID appears at the end of the URL for the page.

    ![Saved query record ID at the end of the page URL](media/custom-view-queryid.PNG "Saved query record ID at the end of the page URL")

## Step 3: Create a Guides view configuration record

The purpose of the configuration record is to notify HoloLens about the view that it should use.

1. Go to [https://powerapps.microsoft.com](https://powerapps.microsoft.com), and sign in as an admin for the instance.

2. In the left pane, select **Apps**, and then select **Guides**. This opens the Guides model-driven app.

    > [!NOTE]
    > The Guides model-driven app is not intended to be a replacement for the PC/HoloLens authoring applications. Be careful when you create, update, or delete records using the Guides model-driven app as it may prevent users from using the PC/HoloLens applications in an intended and supported way (for example, whether a guide can be opened correctly in the applications).

    ![Select Guides](media/custom-view-apps-guides.PNG "Select Guides")

3. In the left pane, under **Configuration**, select **Guides View**, and then select **New**.

    ![Create a Guides view record](media/custom-view-configuration-guides-view.PNG "Create a Guides view record")

4. On the **New Guide View Configuration** page, enter a name that will help you remember what this configuration record is for. This name isn't used for the tab name on HoloLens.

    ![Enter a record name](media/custom-view-name-guides-configuration.PNG "Enter a record name")

5. In the **Saved Query ID** field, enter the record ID that you saved in step 8 in the previous section. This value isn't validated. Therefore, copy it carefully to ensure that it's correct.

    ![Enter the saved query record ID](media/custom-view-saved-queryid.PNG "Enter the saved query record ID")

6. Select **Save and Close**.

> [!WARNING]
> There is no relationship between the Guide view configuration record and the saved view. If you delete the target view or entity, a fetch of the data will fail, and data won't be shown on HoloLens.

## Step 4: Use the App Designer to add specific guides to the list that is shown in the view

In this step, you will add the list of guides that will appear on the HoloLens tab.

> [!NOTE]
> The following procedure is an example that shows how to use the App Designer. You can configure the App Designer in different ways, depending on your experience with Dynamics 365.

1. Go to [https://powerapps.microsoft.com](https://powerapps.microsoft.com), and sign in as an admin for the instance.

2. In the left pane, select **Apps**. Then select the **More Commands** (**...**) button next to **Guides**, and select **Edit**.

    ![Edit the Guides app](media/custom-view-guides-edit-button.PNG "Edit the Guides app")

3. In the App Designer, select the **Edit** button (pencil symbol) next to **Site Map**.

    ![Edit button for Site Map](media/custom-view-sitemap-edit.PNG "Edit button for Site Map")

4. Select the **Configuration** heading, select **Add**, and then select **Group**.

    ![Add a group](media/custom-view-add-group.PNG "Add a group")

5. Enter a name for the new group (for example, **Custom Tab**). This name will appear to the right of the other headings on the **Sitemap Designer** page.

6. Select the heading for the new group, select **Add**, and then select **Subarea**.

    ![Add a subarea](media/custom-view-add-subarea.PNG "Add a subarea")

7. On the **Properties** tab on the right side of the page, in the **Entity** field, select the name of the entity that you created in the [Step 1: Create a new entity in Common Data Service](#step-1-create-a-new-entity-in-common-data-service) section. In this way, you link the subarea.

    ![Link the subarea](media/custom-view-link-subarea.PNG "Link the subarea")

8. In the upper-right corner of the page, select **Save**, and then select **Publish**.

9. In the upper-left corner of the page, select **App Designer** to return to the App Designer.

10. Scroll down to the **Forms** item for your entity, and select it.

    ![Select the Forms item for the entity](media/custom-view-select-forms.PNG "Select the Forms item for the entity")

11. On the **Components** tab on the right side of the page, in the **Main Forms** section, select the **Edit** button (pencil symbol).

    ![Edit button](media/custom-view-edit-main-form.PNG "Edit button")

12. Drag the **Date and Time** and **Guide** fields from the list of fields in the left pane to the center of the page.

    ![Drag the fields](media/custom-view-drag-drop-fields.PNG "Drag the fields")

13. Go to [https://powerapps.microsoft.com](https://powerapps.microsoft.com). You should see your new group and view at the bottom of the left pane.

    ![New group and view in the left pane](media/custom-view-custom-tab-configuration.PNG "New group and view in the left pane")

14. Select the view to open it, and then, in the **Guide** field, select a guide to add to the list.

    ![Add a guide to the list](media/custom-view-select-list.PNG "Add a guide to the list")

    > [!IMPORTANT]
    > When you add a guide to the list, you must specify a date. This date must be either the current date or a future date. Otherwise, the guide won't appear on the custom tab.

15. In the **Owner** field, assign the user who will have access to the list.

16. To add more guides to the list, select **New**, and then set the **Guide** and **Owner** fields again.
