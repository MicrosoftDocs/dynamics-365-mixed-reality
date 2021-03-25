
# Workflow example 3: Collect data on which responses are selected in a non-linear guide created in Dynamics 365 Guides

If you have created a branching guide in Microsoft Dynamics 365 Guides, you can collect the data on which branches are selected by the operator. For example, you might have a branching guide that provides three choices, based on a gauge temperature reading. 

SCREEN SHOT GOES HERE

You can count the number of times the Step ID for each branching option is selected to know how often a particular issue occurs. 

## What you’ll learn in this example

- Find the Step ID for a destination step

- Export the event data for a guide to Microsoft Excel and match it to Step ID data 

- Set up a condition in Microsoft Power Automate to export the event data for a guide to a particular column in a Microsoft Excel spreadsheet

**Estimated time to complete:** 10 minutes for either workflow solution

## Two ways to collect branching data

You can collect branching data in two different ways:

- After the guide event (branch selection) has been executed 

- In real time with Microsoft Power Automate as the event is executed
 
You’ll need to get the Step ID for each destination step, regardless of which method you choose. This tutorial shows you how to get the Step ID and how to use the Step ID for either scenario.

## Get the Step ID for a destination step

You can use the Guides model-driven app to get the Step ID for a destination step.

1. Go to [make.powerapps.com](make.powerapps.com). 

2. Select **Apps**, and then select **Guides**.

     SCREEN SHOT GOES HERE
  
3. Select the appropriate guide in the list. 

     SCREEN SHOT GOES HERE
  
4. Select the **Steps** entity to display the step information for the guide. 

    For this example, we have a question step and three destination steps.

     SCREEN SHOT GOES HERE 
 
    To get the Step ID for a destination step, double-click the step in the model-driven app. The Step ID appears at the end of the page url in the resulting screen.

     SCREEN SHOT GOES HERE
  
## Collect branching data after the event has been executed

1. Copy the Step ID for each destination step into an Excel spreadsheet. The spreadsheet will look something like this when you’re done:
 
    SCREEN SHOT GOES HERE
 
2. Use the model-driven app to export the guide event data.  

    SCREEN SHOT GOES HERE
 
3. Parse the **Payload** column in the exported spreadsheet to check for the Step ID's. For example, the following Excel formula compares the event data in the exported **Active Guide Events** spreadsheet to the Step IDs copied in the first step of this procedure. The formula returns a 1 if it matches an ID or a 0 if it doesn’t.

    =IF(ISNUMBER(SEARCH(B$2,'Active Guide Events'!L2)),1,0) 
 
    The parsed and summed spreadsheet data looks something like this.
 
    SCREEN SHOT GOES HERE

## Collect branching data in real time by using Power Automate

Collecting branching data in real time by using Power Automate requires four steps:

1. Create an Excel spreadsheet with the appropriate columns

2. Create a Power Automate flow that:

    - Is triggered when the guide event is created (when a user selects a destination step).

    - Sets a condition for the guide event Payload field that contains the Step ID. 

    - Writes the date to the Excel spreadsheet. 
 
## Create the spreadsheet

Create an Excel spreadsheet with columns that match your destination steps and a column to record the date/time the branch was selected. For example, for the temperature gauge guide, the spreadsheet would include these four columns: 

- Date 

- 150 to 200 degrees

- 200 to 250 degrees

- 250 to 300 degrees

## Create the flow

1. Sign in to [Power Automate](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fus.flow.microsoft.com%2F&data=04%7C01%7Cv-bholmes%40microsoft.com%7C73759d057d0d49141b2e08d8e3556327%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637509303168916711%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&sdata=hiyg2fP9dF9NgBKNX4e9afLf44Th4vWPaIpAoxW9qfs%3D&reserved=0).
	
2. Select **Create**, and then select **Automated cloud flow**.

    SCREEN SHOT GOES HERE
 
3. Give your flow a name, select the **When a record is created** trigger, and then select **Create**.

    SCREEN SHOT GOES HERE
 
    > [!TIP]
    > You can filter the list of triggers to just the Common Data Service triggers by entering the word **data** in the **Choose your flow’s trigger** box.

4. In the **When a record is created** trigger, select your environment, select **Guide Step Session Visits** for the **Entity Name** field, and then select a scope. 
 
    SCREEN SHOT GOES HERE
    
5. Select **New step**, and then select **Condition**.

    SCREEN SHOT GOES HERE

6. In the **Condition**, create a condition where the **Payload** field contains a destination Step ID. 

    SCREEN SHOT GOES HERE
 
7. In the **If yes** box for the condition, select the **Excel Online (Business)** category, and then select the **Add a row into a table** action.

    SCREEN SHOT GOES HERE

8. Fill out the fields for the **Add a row into a table** action. For example, for the temperature gauge guide, select/enter the following data.

    |Field|	Value|Description|
    |---------------------------|------------------------------|------------------------------------|
    |**Location**|	OneDrive for Business	Cloud location for the file.| You can select OneDrive for Business or a SharePoint site
    |**Document Library**	|OneDrive	|The library for the cloud location|
    |**File**	|**Guides Branching Data.xlxs**|The name of your Excel file|
    |**Table**|	Table 1|???Fill this in???|
    |**Date**|	Created On field (you can select this value dynamically after you place the cursor in the field)	|Records the date and time when the selection was made in the branching guide|
    |**150 to 200 degrees**|1	|Column in the Excel spreadsheet. Enter a **1** if the column aligns with the Step ID in the condition or a **0** if it doesn’t.|
    |**200 to 250 degrees**|0	|Column in the Excel spreadsheet. Enter a **1** if the column aligns with the Step ID in the condition or a **0** if it doesn’t.|
    |**250 to 300 degrees**|0	|Column in the Excel spreadsheet. Enter a **1** if the column aligns with the Step ID in the condition or a **0** if it doesn’t.|

    The following screen shot shows the fields filled in for the Temperature gauge guide. 

    SCREEN SHOT GOES HERE
 
    This condition gets the Step ID for the **150 to 200 degrees** step and puts a 1 in the **150 to 200** column in the Excel spreadsheet when the **Payload** field contains that Step ID.
 
    SCREEN SHOT GOES HERE
 
    You can then tabulate, graph, and analyze the data in Excel.

### Test the flow

1. Select **Save** in the upper-right corner of the screen.

2. To test the flow, in the upper-right corner of the screen, select **Test**, select **Manually**, and then select **Test**. 

    SCREEN SHOT GOES HERE
 
3. In the **Run flow** pane, select **Run flow**. 



