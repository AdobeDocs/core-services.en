---
description: Learn how to validate the [!DNL Customer Attributes] schema in Adobe Experience Cloud.
solution: Experience Cloud
title: How to Validate the [!DNL Customer Attributes] Schema 
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 776d1fd3-c733-4970-a76b-4c3c0119ee77
---
# Validate the schema

The validation process lets you map display names and descriptions to uploaded attributes (strings, integers, numbers, and so on). 

A schema is created based on these settings. The schema is used to validate all future data uploaded to this data source. The mapping process does not alter the original data.

>[!NOTE]
>
>Updating the schema after validation deletes customer attributes. See [Update the schema (also deletes attributes)](t-crs-usecase.md).

**To validate the schema**

1. In [!DNL Customer Attributes], click the attribute source to edit. 

1. On the **[!UICONTROL Edit Customer Attribute Source]**, click **[!UICONTROL File Upload]**.

1. On the [!UICONTROL File Upload and Schema Validation] page, click **[!UICONTROL Actions]** > **[!UICONTROL View/Edit Schema]**

   ![Edit a schema](assets/view_edit_schema.png)

   On the [!UICONTROL Edit Schema] page, each row of the schema represents a column of the uploaded CSV file.

   ![Edit schema page in Experience Cloud](assets/edit-schema.png)

**Actions**

* **[!UICONTROL Add Data:]** Upload new attribute data to this data source.

* **[!UICONTROL View/Edit Schema:]** Map display names to the attribute data, as described in the next step.

* **[!UICONTROL FTP Setup:]** Create your FTP account to [upload your data via FTP](t-upload-attributes-ftp.md) (optional).

* **[!UICONTROL ID Lookup:]** Enter a customer ID (CID) from your `.csv` to look up Experience Cloud information for the ID. This feature is useful for troubleshooting why attribute data is not displaying for a visitor:

  * **[!UICONTROL ECID (Experience Cloud ID):]** Displays if you are using the latest Experience Cloud ID Service. If you are on the MCID service but no IDs are listed here, Experience Cloud has not received an alias for that CID. Meaning, the visitor has not logged in, or your implementation is not passing that ID through.
      
  * **[!UICONTROL CID (customer ID):]** The attributes associated with this CID. If you are using a prop or eVar to upload CIDs (AVID), and you see attributes displayed but no AVID, this indicates that the visitor has not logged in to your site.
      
  * **[!UICONTROL AVID (Analytics visitor ID):]** Displays if you use a prop or eVar to upload CIDs. If those IDs are being passed to Experience Cloud, any visitor IDs associated with the CID you entered are displayed here.
