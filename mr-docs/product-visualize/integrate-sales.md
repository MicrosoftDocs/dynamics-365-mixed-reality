---
author: sbmjais
description: Instructions for integrating Dynamics 365 Sales with Dynamics 365 Product Visualize Hub
ms.author: shjais
ms.date: 07/29/2020
ms.topic: article
title: Integrate Dynamics 365 Sales with Dynamics 365 Product Visualize Hub
manager: shujoshi
---

# Integrate Dynamics 365 Sales with Dynamics 365 Product Visualize Hub

[!INCLUDE [cc-beta-prerelease-disclaimer](../includes/cc-beta-prerelease-disclaimer.md)]

New entities are introduced in Product Visualize Hub to provide your business with the flexibility it needs to use Product Visualize in a variety of scenarios. For the existing Product Visualize users or anyone new to Dynamics 365 Sales, we recommend connecting the Product Visualize entities to the existing Opportunity and Product entities you already use. This will let you quickly transition to the new Product Visualize workflow without significantly changing how your salespeople work. 

This topic guides you through the steps to setup Product Visualize for a standard Dynamics 365 Sales scenario and assumes you already have Dynamics 365 Sales enabled. The same steps could be used to customize any existing Dynamics 365 entities, or even your own custom entities. For this example, we will add the Mixed Reality Session entity to the main form of the Opportunity entity.

## Using web client

1. Open a web browser, and enter the URL to your Dynamics 365 instance in the following format: &lt;domain\_name&gt;.crm.dynamics.com. For example, `https://productvisualize.crm.dynamics.com`

2. Enter your Dynamics 365 instance credentials, and sign in to see a list of published apps. The **Sales Hub** app must be listed to continue.

    ![Apps list](media/apps-list.png "Apps list")

3. Select the **Settings** icon, and then select **Advanced Settings**.

    ![Advance settings](media/advance-settings.png "Advance settings")

    The **Business Management** page opens in a new browser tab.

4. On the navigation bar, select **Settings**, and then under **Customization**, select **Customizations**.

5. Select **Customize the System**.

6. Under **Components** in the solution explorer, expand **Entities**, then expand an entity to you want to connect to, and then select **Forms**. For example, **Entities** > **Opportunity** > **Forms**.

    ![Expand an entity and select Forms in the solution explorer](media/opportunity-forms.png "Expand an entity and select Forms in the solution explorer")

7. Select the main form to open it.

    ![Select the main form](media/select-default-form.png "Select the main form")

8. In the **Field Explorer** pane, select **New Field**.

    ![New field button in Field Explorer](media/new-field-button.png "New field button in Field Explorer")

9. Enter the required details for the new field and select **Save and Close**.

    ![Enter details for the new field](media/new-field-details.png "Enter details for the new field")

10. Go the entity's form you opened in step 7 and refresh the page. The new field is displayed in the **Field Explorer** pane.

    ![New field displayed in Field Explorer](media/new-field-created.png "New field displayed in Field Explorer")

11. Select the field and drag it to the desired location on the form.

    ![Add new field to the form](media/new-field-added-form.png "Add new field to the form")

12. Save and publish the changes.

13. Open Sales Hub, and select **Opportunities** in the left pane.

14. Edit an existing opportunity or create a new opportunity.

15. In the **Mixed-reality session** field, search for the mixed-reality session to link and select it.

    ![Use the new field added to enter data](media/use-new-field.png "Use the new field added to enter data")

16. Follow steps 6 through 15 to add and link to other Product Visualize entities.

## Using new experience

1. Open a web browser, and enter the URL to your Dynamics 365 instance in the following format: &lt;domain\_name&gt;.crm.dynamics.com. For example, `https://productvisualize.crm.dynamics.com`

2. Enter your Dynamics 365 instance credentials, and sign in to see a list of published apps. The **Sales Hub** app must be listed to continue.

    ![Apps list](media/apps-list.png "Apps list")

3. Select the **Settings** icon, and then select **Advanced Settings**.

    ![Advance settings](media/advance-settings.png "Advance settings")

    The **Business Management** page opens in a new browser tab.

4. On the navigation bar, select **Settings**, and then under **Customization**, select **Customizations**.

5. Select **Customize the System**.

6. Select **Try new experience** on the notification bar.

    ![Try new experience](media/try-new-experience.png "Try new experience")

7. In the left pane, expand **Data** and select **Entities**.

    ![Expand Data and select Entities in the left pane](media/left-pane-entities.png "Expand Data and select Entities in the left pane")

8. In the search box at the upper-right corner, search for the entity, and then select it. For example, Opportunity. 

    ![Search and select the Opportunity entity](media/select-opportunity-entity.png "Search and select the Opportunity entity")

9. Go to the **Forms** tab, and select the main form to open it.

    ![Select main form](media/entity-main-form.png "Select main form")

10. In the **Fields** pane, select **New field**.

    ![New field button on the Fields pane](media/new-field-button-pane.png "New field button on the Fields pane")

11. In the **New Field** panel, enter the required details for the new field and select **Done**.

    ![New field details](media/field-details.png "New field details")

12. In the **Fields** pane, search for the new field added.

    ![Search for the new field](media/search-new-field.png "Search for the new field")

13. Select the field and drag it to the desired location on the form.

    ![New field added to the form](media/new-field-added-opp-form.png "New field added to the form")

14. Save and publish the changes.

15. Open Sales Hub, and select **Opportunities** in the left pane.

16. Edit an existing opportunity or create a new opportunity.

17. In the **Mixed-reality session** field, search for the mixed-reality session to link and select it.

    ![Use the new field added to enter data](media/use-new-field.png "Use the new field added to enter data")

18. Follow steps 10 through 17 to add and link to other Product Visualize entities.



[!INCLUDE[footer-include](../includes/footer-banner.md)]
