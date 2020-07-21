

# Migrate Dynamics 365 Guides content from one Common Data Service instance to another using the Content Migration Tool (public preview)

The Content Migration Tool (Public Preview) for Dynamics 365 Guides is a [PowerShell](https://docs.microsoft.com/windows-server/administration/windows-commands/powershell) script that copies content from one Common Data Service instance to another. You can migrate all the content in an instance or just specific types of content (for example, 3D objects, images, and videos). After migrating, the content will exist in both instances. The content in the source instance is not changed in any way.

The tool connects to two Common Data Service instances at once. It reads the content in the source instance and writes it to the destination instance. The instances can be part of the same tenant or can be in different tenants. 

> [!NOTE]
> By using the Content Migration Tool (Public Preview) for Dynamics 365 Guides, you acknowledge and accept all the limitations of using a preview tool, including that the terms and commitments for Dynamics 365 Guides and other Microsoft commercial services and products do not apply to the Migration Tool. You also assume all risks associated with migrating your data between Dynamics 365 tenants, including but not limited to risks of different security, compliance, and privacy commitments, and damage to or loss of data, and unavailability or interruption of the tool.

The tool supports the following types of migrations. 

|Type of migration|What's migrated?|
|------------------------------------------------------|------------------------------------------------------------------|
|All content|	Everything stored in the instance that’s active (excludes telemetry events associated with a guide).|
|Guides and associated content|	Active guides and any 3D objects, images, or videos related to those guides. Inactive content associated with a guide is also migrated. You can choose to migrate all existing guides at once or select specific guides. |
|All 3D objects, images, and videos|	All active 3D objects, images, and videos stored in the instance.|
|Only 3D objects|Active 3D objects only. You can choose to migrate all existing 3D objects at once, migrate all 3D objects that belong to a 3D object collection, or select specific 3D objects. |
|Only images|Active images only. You can choose to migrate all existing images at once or select specific images.|
|Only videos|Active videos only. You can choose to migrate all existing videos at once or select specific videos.|

>[!NOTE]
>-[Website and Power Apps links](pc-app-website-powerapps-link.md) are migrated when you migrate the guides. However, for Power Apps, you’ll also need to manually import the apps into the new instance and update the links in the steps.<br><br>- Migration of guides based on schema v3 is not supported by this tool. If you have updated your Dynamics 365 Guides solution to the latest version and still have a guide based on schema v3, you can [do a manual upgrade](https://docs.microsoft.com/dynamics365/mixed-reality/guides/upgrade#troubleshooting-you-receive-a-guide-cannot-be-opened-error-message).<br><br>- For 3D objects that belong to a 3D object collection, the parent 3D object will not be migrated unless you have the **System Admin** role.

## Prerequisites

- You must have a Dynamics Insider Program account to have access to the download files. 

- You must be a system administrator for the PC you use to run the PowerShell script. 

- You must use [PowerShell](https://docs.microsoft.com/powershell/scripting/install/installing-windows-powershell?view=powershell-7#how-to-check-the-version-of-powershell) version 5.1.18362.752 or later. 

- Both the source instance and destination instance must use Dynamics 365 Guides solution version 400.0.0 or later. 

- You must have credentials to sign in to the source instance with the **System Admin** role (preferable) or **Operator/Author** role (required).  

- You must have credentials to sign in to the destination instance with the **System Admin** role (preferable) or **Author** role (required). 

We also highly recommend [backing up the contents](https://docs.microsoft.com/power-platform/admin/backup-restore-environments#create-a-manual-backup) of both instances before starting the migration process. 

>[!NOTE]
>Multi-factor authentication is not supported by this tool.







