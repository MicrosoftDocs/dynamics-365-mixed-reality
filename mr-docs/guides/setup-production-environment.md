

# Set up a production environment for Dynamics 365 Guides

1.	Go to the [Power Platform Admin center](https://admin.powerplatform.microsoft.com/environments), select **Environments** if it's not already selected, and then select **New**.

    ![Add new environment](media/add-new-environment.PNG "Add new environment") 

    The **New enironment** pane appears on the right side of the screen.

    ![New environment pane](media/new-environment-pane.PNG "New environment pane") 

3.	In the **New environment** pane:

    a.	Enter a name for the environment.

    b.	In the **Type** list, select **Production**.

    c.	In the **Region** field, keep the default setting.  

    d.	In the **Create a database for this environment?** field, move the slider to **Yes**.

    e.	Select **Next** at the bottom of the screen. 

3. In the **Add database** pane that appears, choose your language and currency, and then select **Save**.

   ![Add database pane](media/add-database-pane.PNG "Add database pane") 

   The following page appears while the production environment is being prepared. 
   
    ![Enviroment getting prepared message](media/environment-message.PNG "Environment getting prepared message") 

4.	After the new environment is active (listed as **Ready** in the **State** column) go to [Change maximum upload file size instructions](https://docs.microsoft.com/dynamics365/mixed-reality/guides/setup#change-maximum-upload-file-size). 

### See also

[Buy and deploy Dynamics 365 Guides](setup.md)
