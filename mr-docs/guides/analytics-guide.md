---
author: BryceHo
description: Covers Guides Analytics--Power BI reports you can use in Dynamics 365 Guides to improve process efficiencies.
ms.author: cynielse
ms.date: 02/02/2021
ms.service: crm-online
ms.topic: article
title: Overview of Guides Analytics, Power BI reports for Dynamics 365 Guides
ms.reviewer: v-brycho
---

# Analyze guides created with Dynamics 365 Guides

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Watch a video on analyzing your guides with Power BI reports](https://aka.ms/guidesanalyze)<br>
 
Guides Analytics is part of the [!include[cc-microsoft](../includes/cc-microsoft.md)] [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] application suite that includes the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC authoring app and the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app. Use Guides Analytics to analyze the usage of guides across your organization. Guides Analytics consists of [!include[pn-power-bi](../includes/pn-power-bi.md)] visual reports that are populated with [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] session data stored securely in your [!include[pn-dyn-365](../includes/pn-dyn-365.md)] environment. 

> [!NOTE]
> Guides Analytics is intended to help supervisors and managers derive insights regarding operational efficiencies and usage of Dynamics 365 Guides. This feature is not intended for use in making (and should not be used to make) decisions that affect the employment of an employee or group of employees, including compensation, rewards, seniority, or other rights or entitlements. Customers are solely responsible for using Dynamics 365, this feature, and any associated feature or service in compliance with all applicable laws, including laws relating to accessing individual employee analytics and monitoring. Customers are encouraged to have a mechanism in place to inform their users that analytics relating to their guides usage is collected.

## What data is collected and used in Guides Analytics? 

When an operator uses the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] [!include[pn-hololens](../includes/pn-hololens.md)] app in Operate mode, each interaction that moves the operator forward, backward, or out of the guide is recorded, together with the date and time of the interaction. Each operation of a guide in [!include[pn-hololens](../includes/pn-hololens.md)] Operate mode, whether completed from beginning to end of the guide or involving just a few steps, is called a *guide session*. Information about the guide session, such as time spent on a step, step number, task number, total operating time, and different options to define completion (was the completion step visited or what percentage of steps did the operator visit) are also recorded. This data is stored in your private and secure [!include[pn-dyn-365](../includes/pn-dyn-365.md)] environment.  

## What can you do with the data? 

One way to interact with the data is to utilize the Guides Analytics reports, and another way is to use [Microsoft Power Automate to automate workflows](https://docs.microsoft.com/power-automate/), for example when a new guide session starts or ends.  

The Guides Analytics reports are designed to help you answer high-level questions about guides usage. For example: 

- How many guides have been used to date? 
 
- Is the number of times a guide is operated per day increasing, decreasing, or remaining stable over time? 

- Which guides take the most time to complete? 

- Are operators completing the guide or only going through half the steps?

You can also use Guides Analytics to drill into detailed time-tracking information at the task and step levels. For example, answer questions such as: 

- Which step of a guide takes the most time? 

- Which step of a guide has the most variability in operator time? 

- Is the amount of operation time equally distributed between tasks?

These reports provide information about operator adoption and usage and give guide authors a data-driven way to improve their 
guides. For example, an author could focus their editing efforts on steps that take a long time to execute or show a high 
degree of variability among operators. These reports are also valuable in training scenarios for both trainers and trainees 
to better understand performance and improvement over time.  

## Open Guides Analytics 

### Set up the latest version of the reports

You can set up latest Guide Analytics reports through the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC authoring app.

> [!NOTE]
> Guides Analytics requires the freely available [Power BI Desktop application](https://powerbi.microsoft.com/get-started/). Talk to your admin if you don't have permission to install [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop on your computer. 

To set up your reports:
 
1.	In the [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] PC authoring app, select the **Analyze** tab, copy the highlighted Instance URL text, and then select **Continue** to go to the [Microsoft Download Center](https://aka.ms/guidesreport). 
   
    ![Analyze tab](media/get-started-analytics.PNG "Analyze tab")      
 
2.	In the [!include[cc-microsoft](../includes/cc-microsoft.md)] Download Center, select **Download**. 

    ![Microsoft Download Center](media/microsoft-download-center.PNG "Microsoft Download Center") 

    You'll be prompted to choose the files to download: 

     - **Guides Analytics Template.** You can configure this [!include[pn-power-bi](../includes/pn-power-bi.md)] template file to display [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] time-tracking data from within your organization. 
   
     - **Guides Analytics Demo.** You can use this [!include[pn-power-bi](../includes/pn-power-bi.md)] file to view an example data set. It does not require any configuration and lets you get an overview of Guides Analytics reports before you even create your first guide.  

     We recommend downloading both files. 

     ![Files to download](media/download-files.PNG "Files to download")   
  
3.	Open the downloaded Guides Analytics Template.pbit file with [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop. Use your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] username and password if you're prompted to sign in to [!include[pn-power-bi](../includes/pn-power-bi.md)].  
 
4.	When prompted, paste the Instance URL into the text box as shown here. This is the same Instance URL you copied from the **Analyze** tab in the PC authoring app in step 1. 

     ![Guides Analytics template](media/guides-analytics-template.PNG "Guides Analytics template")
 
     You might see the following error message saying you aren't signed in: 
  
     ![Sign-in error](media/sign-in-error.PNG "Sign-in error")

     In that case, select **Sign in**, and enter your [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] username and password to connect the template to your organization's secure [!include[pn-dyn-365](../includes/pn-dyn-365.md)] environment. 

5.	You should now see the template populated with data from your own guides. If you haven't operated any guides yet, your reports might appear blank. The reports are described in detail in "Take a tour of reports" later in this topic. 
 
     ![Example report](media/example-report.PNG "Example report")
 
6.	Save the configured reports to a convenient place on your computer for later use. 

7.	Select **Refresh** on the **Home** ribbon to update your reports with the most recent [!include[pn-dyn-365-guides](../includes/pn-dyn-365-guides.md)] data. 
 
### Open your reports 

Once you have set up and saved the Guides Analytics Template on your computer, open [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop, and then open your saved report. [!include[pn-power-bi](../includes/pn-power-bi.md)] Desktop has a **File – Open – Recent** items list that's convenient for finding your previously opened reports.  

## Take a tour of reports 

Both the Guides Analytics Template and Guides Analytics Demo files contain two reports: Guides Usage and Process Time-Tracking.

### Guides Usage report

The Guides Usage report provides an overview of all the guides used in your organization. The following graphic illustrates the parts of the report.

![Guides Usage report](media/guides-usage-report.PNG "Guides Usage report") 
 
1.	Which guides are included in the report?

    Use the drop-down menu to select which guides are used to generate the visuals and statistics in the report. Changing the selection in this drop-down menu changes the values in all parts of the report. By default, the **All** option is selected to give you an overview of all your organization's guides.
   
2.	Use the summary statistics to quickly answer the following questions:

    - **Guides.** How many guides have been used by at least one operator to date? 
   
    - **Users.** How many users have operated at least one guide to date? 
   
    - **Sessions.** How many sessions have been completed to date? 
   
3.	Is daily guide usage changing? 

    The bar chart of session counts (y-axis) per day (x-axis) allows you to see trends such as increasing, decreasing, or stable daily guides usage. 
    
    > [!TIP]
    > Use drill up/drill down. By default, this chart shows the session counts per day. However, you can use Power BI’s drill-up functionality to summarize session counts at the month or year level. [Learn more about how to use Drill mode in a Power BI visual](https://docs.microsoft.com/power-bi/consumer/end-user-drill).   

4.	Which guides have the most sessions, longest or shortest session times, or were operated most recently? 

    This table displays the following information per guide: current number of tasks and steps, the latest start time, the total number of sessions, as well as the maximum and minimum session time observed to date. By default, this table is sorted by guide name, but you can select a column header to sort by that field. For example, select **Max session time** to quickly find which guide has the longest session time. 
       
5.	Filters. There are situations in which you might want to filter the report to show just a subset of sessions. For example:

    - **Filter on a date range.** The date filter is useful for exploring guides usage on a particular date or across a time window of interest.

    - **Filter on completion status.** There are many ways to define whether a guide session is “complete”. For example, it may be important that the operator visited a completion step. Alternatively, you may want to check that a minimum percentage of steps were visited in the session. You can filter on these items separately or together. 

    - **Filter on role.** In most cases, you’ll want to filter guides by Operator role. You may want to filter by Author when you’d like to see data from sessions where an Author is previewing their guide and experiencing it as an operator would.    
    
> [!IMPORTANT]
> If sessions have any missing data, they're not included in the Guides Analytics reports. For example, sessions that are currently in progress or that are comprised solely of visits to the alignment step will not be included. On rare occasions, session data can be lost due to connectivity or other technical issues, resulting in one or more step visits not being correctly recorded or the guide session being interrupted. In these cases, the session is excluded from the reports.

### Process Time-Tracking report

Use the Process Time-Tracking report to analyze step-level run-time data for a single guide. The following graphic illustrates the parts of the report.

![Process Time-Tracking report](media/process-time-tracking-report.PNG "Process Time-Tracking report")
 
1.	Which guides are included in the report?

    Use the drop-down menu to select a single guide. Changing the selection in the drop-down menu changes the values in all 
   parts of the report to correspond to data for that single guide. 
   
2.	Use the summary statistics to quickly answer the following questions: 

    - **Users.** How many users have operated this guide at least once? 
   
    - **Sessions.** How many total sessions of this guide have been completed to date? 
    
    - **Avg. Session Time.** What is the average session time for this guide?
   
3.	How long are individual steps on average? 

    This table shows you the task and steps for the selected guide. You can select the average step time or standard deviation columns to quickly find the longest/shortest steps or steps with most/least variability in time (standard deviation). If a step is visited multiple times in the same session, the total time spent on that step will be used in the step average calculation. If a step is visited multiple times in the same session, the total time spent on that step will be used in the step average calculation. Select a row of this table to filter all the visuals in the report to just that step.
    
    Note that the report does not provide times for alignment and completion steps.
    
    > [!TIP]
    > - To sort by multiple columns, hold the Control key down while you select to add another column to the sort order. This is useful if you want to sort by task and step number. [Learn more about how to change the sort order in a Power BI report](https://docs.microsoft.com/power-bi/consumer/end-user-change-sort).   
    > - To use multiple rows as filters, hold down the Shift key while you select each row. [Learn more about how to multi-select data elements in Power BI Desktop](https://docs.microsoft.com/power-bi/create-reports/desktop-multi-select).
   
4.	Which sessions are the longest/shortest? 

    This table shows all the operator sessions for the selected guide. It includes information about each session’s total time, the percentage of all steps in the guide that were visited at least once, and whether or not at least one completion step was visited. This table is helpful for finding the longest/shortest sessions or investigating the completion status of individual sessions. Select a row of this table to filter all the visuals in the report to just that session.
See the tips in the previous step for sorting by multiple columns or using multiple rows as filters.
   
5.	How long did each task or step take? 

    This dot plot shows the time in minutes (y-axis) for each step of a guide (x-axis) to give you a sense for which steps take the most time and which steps have the most variability in time. If a step is visited multiple times in the same session, the sum of the step visit times is displayed. Each guide session is shown in a separate color. Sessions may have the same color if there are many sessions displayed. 
    
    ![Dot plot showing how long each step takes](media/process-time-tracking-report-session-time.PNG "Dot plot showing how long each step takes")   
    
    > [!TIP]
    > - Use drill up/drill down. By default, this chart shows the time per step. However, you can use Power BI’s drill-up functionality to summarize time at the task level. [Learn more about how to use Drill mode in a Power BI visual](https://docs.microsoft.com/power-bi/consumer/end-user-drill).
    > - Add a constant line. To easily compare step times to a standard target time, you can add a constant line to your step time dot plot. [Learn more about how to use the Analytics pane in Power BI](https://docs.microsoft.com/power-bi/transform-model/desktop-analytics-pane).      
   
7.	Filters. There are situations in which you might want to filter the report to show just a subset of sessions. For example: 
   
     - **Compare versions of a guide.** The date filter is particularly useful if you made a revision to your guide (for example, added 
   or removed a step) and you want to show data for a given version of the guide that can be identified based on the date the guide 
   was created or edited. 
   
    - **Filter on completion status.** There are many ways to define whether a guide session is “complete”. For example, it may be important that the operator visited a completion step. Alternatively, you may want to check that a minimum percentage of steps were visited in the session. Guides provides these measures and you can use them separately or together to filter sessions in the Process Time-Tracking report. 
   
    - **Filter on role.** In most cases, you’ll want to filter guides by Operator role. You might want to filter by Author when you’d like to see data from sessions where an Author is previewing their guide and experiencing it as an operator would.

     - **Filter out the outliers.** Unusually long step times can stretch the y-axis of the time-per-step line chart, which can make the 
   majority of data difficult to see. Use this slider to set the range of step times you want to visualize across the report so you 
   can ignore the outliers.  
   
> [!IMPORTANT]
> If sessions have any missing data, they're not included in the Guides Analytics reports. For example, sessions that are currently in progress or that are comprised solely of visits to the alignment step will not be included. On rare occasions, session data can be lost due to connectivity or other technical issues, resulting in one or more step visits not being correctly recorded or the guide session being interrupted. In these cases, the session is excluded from the reports.

## Share the Guides Analytics reports 

If you have a [!include[pn-power-bi](../includes/pn-power-bi.md)] Pro license, you can share your Guides Analytics [!include[pn-power-bi](../includes/pn-power-bi.md)] reports within your organization by publishing them to the [!include[pn-power-bi](../includes/pn-power-bi.md)] Service. This allows anyone in your organization with a [!include[pn-power-bi](../includes/pn-power-bi.md)] Pro license to access the report through the [!include[pn-power-bi](../includes/pn-power-bi.md)] Service web interface accessible at https://powerbi.microsoft.com.

Once you have a [!include[pn-power-bi](../includes/pn-power-bi.md)] Pro license, there are several mechanisms for sharing reports with others in your organization. We recommend reading [Ways to share your work in Power BI](https://docs.microsoft.com/power-bi/service-how-to-collaborate-distribute-dashboards-reports) for an overview. A great way to share your reports within your organization in a read-only fashion is to publish them as a [!include[pn-power-bi](../includes/pn-power-bi.md)] app. This involves the following well-documented steps:

1.	[Create a workspace in the Power BI Service](https://docs.microsoft.com/power-bi/service-create-workspaces). 

2.	[Publish your Guides Analytics reports to this workspace using Power BI Desktop](https://docs.microsoft.com/power-bi/desktop-upload-desktop-files). 

3.	[Publish the contents of your workspace as an app in the Power BI Service](https://docs.microsoft.com/power-bi/service-create-distribute-apps).  
 
## See also

![Video camera graphic](media/video-camera.PNG "Video camera graphic") [Analyze your guides](https://aka.ms/guidesanalyze)<br>
![Doc graphic](media/doc-icon.PNG "Doc graphic") [Overview of authoring a guide](authoring-overview.md)</br>
![Doc graphic](media/doc-icon.PNG "Doc graphic") [Overview of operating a guide](operator-overview.md)</br>
![Doc graphic](media/doc-icon.PNG "Doc graphic") [FAQ](faq.md)



