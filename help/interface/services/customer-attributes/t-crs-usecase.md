---
description: Create a customer attribute source and upload it to the Adobe Experience Cloud.
solution: Experience Cloud
title: Create a customer attribute Source and Upload the Data File 
uuid: 53dca789-9a91-4385-839d-c9d1aa36b9be
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 21ed7c35-aac9-46f1-a50c-84e7c075209c
---
# Create a customer attribute source and upload the data file

Create the customer attribute source (`.csv` and `.fin` files) and upload the data. You can activate the data source when you are ready. After the data source is active, share the attribute data to Analytics and Target. 

## customer attributes workflow {#concept_BF0AF88E9EF841219ED4D10754CD7154}

![customer attributes workflow](assets/crs.png) 

>[!IMPORTANT]
>
>To access this feature, users must be assigned to the customer attributes product profile (customer attributes - Default Access). Navigate to **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. If *customer attributes* displays as one of the [!UICONTROL product profiles], you are ready to begin. Users that are added to the customer attributes group sees the [!UICONTROL customer attributes] menu on the left side of the Experience Cloud interface. 
>
>To use the customer attributes feature, users must also belong to application-level groups (Adobe Analytics or [!DNL Target]). 

## Create a data file {#create-data}

This data is enterprise customer data from your CRM. The data might include subscriber data for products, including member IDs, entitled products, most-launched products, and so on.

1. Create a `.csv` file.

   >[!NOTE]
   >
   >Later in this process, you drag and drop the `.csv` file to upload the file. However, if you [upload via FTP](t-upload-attributes-ftp.md#task_591C3B6733424718A62453D2F8ADF73B), you also need a `.fin` file with the same name as the `.csv`. 

   Sample enterprise customer data file: 

   ![Sample enterprise customer data file](assets/01_crs_usecase.png) 

1. Before continuing, review the important information in [Data File Requirements](crs-data-file.md), before you upload the file.
1. [Create a customer attribute source and upload the data](t-crs-usecase.md), described below.

## Create the attribute source and upload the data file {#create-source}

Perform these steps on the Create new customer attribute source page in Experience Cloud.

>[!IMPORTANT]
>
>When creating, modifying, or deleting customer attribute sources, there is a delay of up to one hour before IDs begin synchronizing with the new data source. You must have administrative rights in Audience Manager to create or modify customer attribute sources. Contact Audience Manager customer Care or consulting to obtain administrative rights.

1. In [!DNL Experience Cloud], select the Menu  ![menu](assets/menu-icon.png) icon.
1. Select **[!UICONTROL customer attributes]**.

   The [!UICONTROL customer attributes] page is where you can manage and edit existing attribute data sources. 

   ![customer attributes main screen](assets/cust-attr.png)

1. Click **[!UICONTROL New]**.

   ![Step Result](assets/04_crs_usecase.png)
 
1. On the [!UICONTROL Create customer attribute Source] page, configure the following fields:

    * **[!UICONTROL Name:]** A friendly name for the data attribute source. For [!DNL Adobe Target], attribute names cannot include spaces. If an attribute with a space is passed, [!DNL Target] ignores it. Other characters not supported include: `< , >, ', "`. 
    
    * **[!UICONTROL Description:]** (Optional) A description of the data attribute source. 
    
    * **[!UICONTROL Alias ID:]** Represents a source of customer attribute data, such as a specific CRM system. [!UICONTROL Alias ID] is a unique ID that is used in your [!UICONTROL customer attribute Source] code. The ID should be unique, lowercase, with no spaces. The value that is entered in the [!UICONTROL Alias ID] field for a customer attribute source in Experience Cloud should match the values that are being passed in from the implementation (whether via Platform Data Collection or JavaScript of the Mobile SDK.) 

      >[!IMPORTANT]
      >
      >Deleting a data source associated with an Alias ID does not make the Alias ID available, as the Alias ID is saved in multiple services and used to map profiles between them.
            
      The Alias ID corresponds to certain areas where you set additional customer ID values. For example: 
    
        * **Tags:** The Alias ID corresponds to the *Integration Code* value under [!UICONTROL customer Settings], in the [Experience Cloud ID Service](https://experienceleague.adobe.com/docs/experience-platform/tags/home.html) tool. 

        * **Visitor API:** The Alias ID corresponds to the additional [customer IDs](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html) that you can associate with each visitor. 
        
          For example, *"crm_id"* in: 
        
          ```
          "crm_id":"67312378756723456"
          ```
       
        * **iOS:** The Alias ID corresponds to *"idType"* in [visitorSyncIdentifiers:identifiers](https://experienceleague.adobe.com/docs/mobile-services/ios/overview.html). 
        
          For example: 
               
          `[ADBMobile visitorSyncIdentifiers:@{@<`**`"idType"`**`:@"idValue"}];` 
        
        * **Android&trade;:** The Alias ID corresponds to *"idType"* in [syncIdentifiers](https://experienceleague.adobe.com/docs/mobile-services/android/overview.html). 
        
          For example: 
        
          `identifiers.put(`**`"idType"`**`, "idValue");`
        
          See [Leveraging multiple data sources](crs-data-file.md#section_76DEB6001C614F4DB8BCC3E5D05088CB) for additional information about data processing regarding the Alias ID field and customer IDs. 

    * **[!UICONTROL Namespace Code:]** Use this value to identify the customer attribute source when using the [IdentityMap](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/identity/overview) as part of an AEP WebSDK Implementation.
        
## Upload file {#upload}


1. Click File Upload.

2. Drag and drop the `.csv` or `.zip` or `.gzip` data file into the drag-and-drop window.
    
  >[!IMPORTANT]
  >
  >Specific data file requirements exist. See [Data File Requirements](crs-data-file.md) for more information. 
    
  After uploading the file, table data is displayed under the [!UICONTROL File Upload] heading on this page. You can validate the schema, configure subscriptions, or set up the FTP. 
    

  ![attributes](assets/file_upload_attributes.png) 
    
* **[!UICONTROL Unique customer ID:]** Displays how many unique IDs you have uploaded to this attribute source. 
    
* **[!UICONTROL customer-Provided IDs Aliased to Experience Cloud Visitor IDs:]** Displays how many IDs have been aliased to Experience Cloud Visitor IDs. 
    
* **[!UICONTROL customer-Provided IDs with High Alias Counts:]** Displays the count of customer-provided IDs with 500 or more aliased Experience Cloud Visitor IDs. These customer-provided IDs most likely do not represent individuals but rather some sort of shared login. The system distributes the attributes associated with these IDs to the 500 most recent aliased Experience Cloud Visitor IDs, until the alias count reaches 10,000. Then, the system invalidates the customer-provided ID and no longer distributes associated attributes. -->
    
## Validate the schema {#validate-schema}

The validation process lets you map display names and descriptions to uploaded attributes (strings, integers, numbers, and so on). You can also delete attributes by updating the schema.

See [Validate the schema](validate-schema.md). 

To delete attributes, see [(Optional) Update the schema (deletes attributes)](t-crs-usecase.md). 

## (Optional) Update the schema (delete attributes) {#task_6568898BB7C44A42ABFB86532B89063C}

How to delete attributes and replace attributes in the schema.

1. On the [!UICONTROL Edit customer attribute Source] page, remove the **[!UICONTROL Target]** or **[!UICONTROL Analytics]** subscription (under [!UICONTROL Configure Subscriptions]).
1. [Upload a new data file with updated fields](t-crs-usecase.md).

## Configure subscriptions and activate the attribute source {#task_1ACA21198F0E46A897A320C244DFF6EA}

Configuring a subscription sets up the data flow between Experience Cloud and applications. Activating the attribute source allows the data to flow to subscribed applications. The customer records you have uploaded are matched up with incoming ID signals from your web site or application.

See [Configure subscriptions](subscription.md). 

**To activate an attribute source** 

On the [!UICONTROL Create New or Edit customer attribute Source] page, locate the [!UICONTROL Activate] heading, then click **[!UICONTROL Active]**.

   ![Step Result](assets/activate_attribute_source.png) 

## Use customer attributes in Adobe Analytics {#task_7EB0680540CE4B65911B2C779210915D}

With the data now available in applications like Adobe Analytics, you can report on the data, analyze it, and take the appropriate action in your marketing campaigns.

The following example shows an [!DNL Analytics] segment based on the uploaded attributes. This segment shows [!DNL Photoshop Lightroom] subscribers whose most-launched product is Photoshop. 

![Analytics segment based on the uploaded attributes](assets/08_crs_usecase.png) 

When you publish a segment to Experience Cloud, it becomes available in Experience Cloud Audiences and Audience Manager. 

## Use customer attributes in Adobe Target {#task_FC5F9D9059114027B62DB9B1C7D9E257}

In [!DNL Target], you can select a customer attribute from the [!UICONTROL Visitor Profile] section when creating an audience. All customer attributes have the prefix `crs.` in the list. Combine these attributes as required with other data attributes to build audiences.

![Use customer attributes in Adobe Target](assets/crs-add-attribute-target.png) 

See [Creating a New Audience](https://experienceleague.adobe.com/docs/target/using/audiences/create-audiences/audiences.html) in [!DNL Target] help.
