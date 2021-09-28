---
author: amaraanigbo
description: Customer Asset Attachment entity.
ms.author: soanigbo
ms.date: 06/09/2020
ms.service: crm-online
ms.topic: article
title: msdyn_customerassetattachment EntityType
ms.reviewer: v-bholmes
---

# msdyn_customerassetattachment EntityType

Namespace: Microsoft.Dynamics.CRM

Dedicated file attachment to a Customer Asset.

Entity Set Path [organization URI]/api/data/v9.0/msdyn_customerassetattachment

Base Type: [crmbaseentity](/dynamics365/customer-engagement/web-api/crmbaseentity?view=dynamics-ce-odata-9)

Display Name: Customer Asset Attachment

Primary Key: msdyn_customerassetattachmentid

Primary Key Attribute: msdyn_name

Operations Supported: POST, GET, PATCH, DELETE

## Properties

Properties represent fields of data stored in the entity. Some properties are read-only.

|Name  |Type   |Details|
|----------|-----------|------------|
|createdon|Edm.DateTimeOffset|Shows the date and time when the record was created. The date and time are displayed in the time zone selected in Microsoft Dynamics 365 options. </br> </br> Display Name: Created On </br></br> Read Only|
|importsequencenumber|Edm.Int32|Shows the sequence number of the import that created this record. </br> </br> Display Name: Import Sequence Number|
|modifiedon|Edm.DateTimeOffset|Shows the date and time when the record was last updated. The date and time are displayed in the time zone selected in Microsoft Dynamics 365 options. </br> </br> Display Name: Modified On </br></br> Read Only|
|msdyn_customerassetattachmentid|Edm.Guid|Shows the entity instances. </br> </br> Display Name: Customer Asset Attachment|
|msdyn_name|Edm.String|Enter the name of the custom entity. </br> </br> Display Name: Name|
|msdyn_attachmenttype|Edm.String|Type of file attachment. </br> </br> Display Name: Attachment Type </br></br> 700610000 (Value) - Image (Label) </br></br> 700610001 (Value) - Video (Label)|
|msdyn_file|Edm.String|Field to attach video to the attachment. </br> </br> Display Name: Video|
|msdyn_image|Edm.String|Field to attach image to the attachment. </br> </br> Display Name: Image|
|msdyn_category|Edm.Int32|Category of attachment. </br> </br> Display Name: Category </br></br> 700610000 (Value) - Capture (Label) </br></br> 700610001 (Value) - Document (Label)|

## Lookup properties

Lookup properties are read-only, computed properties which contain entity primary key Edm.Guid data for one or more corresponding single-valued navigation properties. More information: [Lookup properties](/dynamics365/customer-engagement/developer/webapi/web-api-types-operations#lookup-properties) and [Retrieve data about lookup properties](/dynamics365/customer-engagement/developer/webapi/query-data-web-api#retrieve-data-about-lookup-properties).

|Name|Single-valued navigation property|Description|
|----------|-----------|------------|
|_createdby_value|createdby|Unique identifier of the user who created the record.|
|_createdonbehalfby_value|createdonbehalfby|Shows who created the record on behalf of another user.|
|_modifiedby_value|modifiedby|Unique identifier of the user who modified the record.|
|_modifiedonbehalfby_value|modifiedonbehalfby|Shows who last updated the record on behalf of another user.|
|_msdyn_customerasset_value|msdyn_customerasset| Reference to Customer Asset associated with the record.|
|_ownerid_value|ownerid|Owner Id|
|_owningbusinessunit_value|owningbusinessunit|Unique identifier for the business unit that owns the record|
|_owningteam_value|owningteam|Unique identifier for the team that owns the record.|
|_owninguser_value|owninguser|Unique identifier for the user that owns the record.|

## Single-valued navigation properties

Single-valued navigation properties represent lookup fields where a single entity can be referenced. Each single-valued navigation property has a corresponding partner collection-valued navigation property on the related entity.

|Name|Type|Partner|
|----------|-----------|------------|
|createdby|[systemuser](/dynamics365/customer-engagement/web-api/systemuser?view=dynamics-ce-odata-9)|lk_msdyn_customerassetattachment_createdby|
|createdonbehalfby|[systemuser](/dynamics365/customer-engagement/web-api/systemuser?view=dynamics-ce-odata-9)|lk_msdyn_customerassetattachment_createdonbehalfby|
|modifiedby|[systemuser](/dynamics365/customer-engagement/web-api/systemuser?view=dynamics-ce-odata-9)|lk_msdyn_customerassetattachment_modifiedby|
|modifiedonbehalfby|[systemuser](/dynamics365/customer-engagement/web-api/systemuser?view=dynamics-ce-odata-9)|lk_msdyn_customerassetattachment_modifiedonbehalfby|
|msdyn_customerasset|[msdyn_customerasset](/dynamics365/customer-engagement/web-api/msdyn_customerasset?view=dynamics-ce-odata-9)|msdyn_msdyn_customerasset|
|ownerid|[principal](/dynamics365/customer-engagement/web-api/principal?view=dynamics-ce-odata-9)|owner_msdyn_customerassetattachment|
|owningbusinessunit|[businessunit](/dynamics365/customer-engagement/web-api/businessunit?view=dynamics-ce-odata-9)|business_unit_msdyn_customerassetattachment|
|owningteam|[team](/dynamics365/customer-engagement/web-api/team?view=dynamics-ce-odata-9)|team_msdyn_customerassetattachment|
|owninguser|[systemuser](/dynamics365/customer-engagement/web-api/systemuser?view=dynamics-ce-odata-9)|user_msdyn_customerassetattachment|

## Operations

The following operations can be used with the msdyn_customerassetattachment entity type.

|Name|Binding|
|----------|-----------|
|GrantAccess|Not Bound|
|IsValidStateTransition|Not Bound|
|ModifyAccess|Not Bound|
|RetrievePrincipalAccess|Not Bound|
|RetrieveSharedPrincipalsAndAccess|Not Bound|
|RevokeAccess|Not Bound|

## Solutions

The following solutions include the msdyn_customerassetattachment entity type.

|Name|Description|
|----------|-----------|
|Remote Assist|Empower technicians to collaborate more efficiently by working together from different locations with Dynamics 365 Remote Assist on HoloLens, Android, or iOS devices.|


[!INCLUDE[footer-include](../includes/footer-banner.md)]
