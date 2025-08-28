---
description: Learn about data file requirements and multiple data sources for uploading data in [!DNL Customer Attributes] to Experience Cloud.
solution: Experience Cloud
title: Customer Attribute Data File and Data Sources 
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: e2dfe10d-7003-4afa-a5e6-57703d74efd4
---
# About data file and data sources for [!DNL Customer Attributes]

Data file requirements and multiple data sources for uploading customer attribute data to Experience Cloud.

You need access to CRM or similar data from your enterprise. The data you upload to Experience Cloud must be a `.csv` file. If you upload via FTP or sFTP, you also upload a `.fin` file. 

[!DNL Customer Attributes] is designed to handle a few files per day. To mitigate the issue of having many small files delaying processing, files sent within 30 minutes of a previous batch from the same organization are routed to a lower-priority queue.

## Allowed file types and naming requirements {#section_6F64FA02ACCC4215B0862CB6A1821FBF}

|File Type|Description|
|--- |--- |
|`.csv`|A comma-separated values file (such as one created in Excel). This file contains the customer attribute data.   Naming requirements: Ensure that file name extensions do not contain white spaces.|
|`.fin`|(Required) The `.fin` file tells the system that you are finished uploading data. The name of the `.fin` file must match the name of the `.csv` file.  Adobe recommends creating an empty text file with a `.fin` extension. An empty file saves space and upload time. **Note:**  Renaming a `.fin` file is not allowed after it is uploaded. The `.fin` file must be uploaded separately and cannot be a renamed, previously uploaded file. After you upload the `.fin` file in the customer attributes FTP, the system retrieves data quickly (within one minute). This differs from other Adobe FTP-based systems, which pick up data less frequently (around once per hour). The `.fin` file is not required when using the drag-and-drop upload method.|
|`.gz` or `.zip`|`.gz` (gzip) or `.zip`  - for compressed files. A `.zip` file cannot contain more than one file in the archive. Naming requirements: The name of the `.zip` or `.gz`  should match the name of the `.csv` file . For example, if your `.csv` file is `crm_small.csv`, the `.zip` file should be `crm_small.csv.zip` . The `.fin` file must match the `.csv`.|


## Requirements for the attribute data files {#section_169FBF5B7BBA47CE825B7A330CF3FE98}

**Example CSV** 

The CSV file must adhere to the following format:

![Requirements for the attribute data files](assets/cvs.png)

The same file viewed in a text editor:

![Requirements for the attribute data files](assets/csv_txt.png)

**Guidelines** 

<table id="table_A9849CC9AA784763921DE057F0F61515"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Item </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Drag-and-drop </p> </td> 
   <td colname="col2"> <p>The drag-and-drop file should be less than 100 MB. </p> <p>The <span class="filepath"> .fin </span> file is not required when using the drag-and-drop upload method. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>customer ID column </p> </td> 
   <td colname="col2"> <p> The first column must be a unique customer ID. The ID used should correspond to the ID that is being passed to the Experience Cloud ID Service. </p> <p>For Analytics, the ID being stored in a prop or eVar. </p> <p>For Target, the setcustomerID value. </p> <p> This customer ID is the unique identifier your CRM uses for each person in your database. The remaining columns are attributes that come from your CRM. You choose how many attributes to upload. </p> <p>Friendly, readable names are recommended for the column headings, but not required. When you validate the schema after upload, you can map friendly names to the uploaded rows and columns. </p> <p> <b>About customer IDs</b> </p> <p>Typically, an enterprise uses a customer ID from a CRM system. This ID is set using the <span class="codeph"> setcustomerIDs </span> call when a person logs in. This ID is also used as the key in the CRM file that is uploaded to Experience Cloud. An <a href="t-crs-usecase.md" format="dita" scope="local"> Alias ID </a> is a friendly name for a data store in Audience Manager, where the alias data is stored. The system sends aliases to this data store (via setcustomerIDs). The CRM file is applied to the data in that data store. </p> <p>For <span class="codeph"> setcustomerIDs </span> information, see <a href="https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html" format="https" scope="external"> customer IDs and Authentication States </a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Subsequent headers and columns </p> </td> 
   <td colname="col2"> <p>Subsequent headers should represent the name of each attribute. </p> <p> These columns should contain customer attributes that come from the CRM. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>attribute limits </p> </td> 
   <td colname="col2"> <p>You can upload hundreds of <span class="filepath"> .csv </span> columns to the customer attribute service in Experience Cloud. However, when configuring subscriptions and selecting attributes, the following limits apply depending on the applications you own: </p> <p> 
     <ul id="ul_2BB85067918D4BB3B59394F3E3E37A6D"> 
      <li id="li_93703988B9934384B4B94A839D028380"> <b>Analytics Standard</b>: 3 total </li> 
      <li id="li_D1E5E7BD24C54591B14D15DE97447835"> <b>Analytics Premium</b>: 200 per report suite </li> 
      <li id="li_8C891FE3D1EF49FA9F81E2E32CD0B9CA"> <b>Adobe Target Standard:</b> 5 </li> 
      <li id="li_2B66D43023F34EA685CE2C38A9250CEA"> <b>Adobe Target Premium:</b> 200 </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Row limits </p> </td> 
   <td colname="col2"> <p>There is no known limit to the number of rows. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Column limits </p> </td> 
   <td colname="col2"> <p>For practicality, limit the number of columns to around 200. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Character limits </p> </td> 
   <td colname="col2"> <p>When creating an Analytics subscription, field lengths for the uploaded files are truncated to 255. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>FTP Guidelines and size limitations </p> </td> 
   <td colname="col2"> <p> 
     <ul id="ul_E157EE6F98914EADA0C103D1D1E705D3"> 
      <li id="li_84FBD455DD164A28AC16F4A5AB19E4B3">Maximum file size limit for FTP is 4 GB for each upload. </li> 
      <li>Minimum file size limit for 10 mb for each upload. </li>
      <li>You can upload one file every half hour. </li>
      <li id="li_B69A20C51D824727AA99C1F6F78537A4"> You should drop your <span class="filepath"> .csv </span> (and <span class="filepath"> .fin </span>) file in the root folder of the FTP site. </li> 
     </ul> </p> <p> <p>Important:  The total allowed space for the FTP account is 40 GB. It is your responsibility to delete processed files. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>File requirements </p> </td> 
   <td colname="col2"> <p> Each attribute source should contain the same number of comma-separated fields. </p> <p> Fields containing a line-break, double-quote, or commas must be quoted. </p> <p> Double-quote characters in a field must be escaped using a backslash (\). </p> <p> Blank columns are stored as <span class="term"> null </span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Multiple files </p> </td> 
   <td colname="col2"> <p>When uploading customer attribute data, if you have several files you want to upload in rapid succession, and especially if the files are large, make certain that the previous file has been processed before uploading the next file. You can monitor this by checking when the previous file has been moved to the processed or failed folder within your [!DNL Customer Attributes] FTP account. </p> <p> Breaking a large file into smaller files and submitting them in rapid succession may actually slow down processing unless you can ensure that each file is processed before submitting the next. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Character Encoding </p> </td> 
   <td colname="col2"> <p>For Japan, UTF-8 is mandatory. </p> </td> 
  </tr> 
   <tr> 
   <td colname="col1"> <p>Historical data </p> </td> 
   <td colname="col2"> <p> customer attributes are tied to the underlying visitor profile in [!DNL Analytics]. As such, [!DNL Customer Attributes] are associated with the visitor for the entire life of that visitor profile in [!DNL Analytics]. This profile includes behavior that occurred before the customer logged in for the first time. </p> <p> If you use the Data Warehouse backfill method, the data is tied to a post_visid_high/low that is based on the Analytics ID (AID). If you are using the Experience Cloud ID Service, the data is tied to a post_visid_high/low that is based on Experience Cloud ID (MID). </p> <p> Note that the Data Warehouse backfill method will no longer be available beginning in October 2022. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Data feeds </p> </td> 
   <td colname="col2"> <p>customer attributes are not available in data feeds. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Using multiple data sources {#multiple}

When creating, modifying, or deleting customer attribute sources, there is a delay around one hour before IDs begin synchronizing with the new data source.

The Alias ID for each customer attribute source must be unique. If you have multiple data sources that use the same ID, they can be set up as follows:

**In VisitorAPI.js or the Experience Cloud ID tool in dynamic tag management:**

Set two customer IDs that correspond to the appropriate data sources:

```
Visitor.setcustomerIDs({ 
     "ds_id1":"123456", 
     "ds_id2":"123456" 
});
```

(See [customer IDs and Authentication States](https://experienceleague.adobe.com/docs/id-service/using/reference/authenticated-state.html) for more information.)

In **[!DNL Experience Cloud]** > **[!DNL Customer Attributes]**:

Create two customer attributes sources using unique alias IDs corresponding to the customer IDs above. Using this method allows the same reference ID to be sent to multiple customer attribute sources.
