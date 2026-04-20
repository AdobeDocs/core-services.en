---
description: Learn how to upload customer attribute data via FTP to Experience Cloud.
solution: Experience Cloud
title: Upload Customer Attribute Data File via FTP
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
TQID: https://experienceleague.adobe.com/jI2dWXMmrrWxceVi-sZtzF5cTF11iy4d7QKkx71vF-I
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: Experience Cloud
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
    internal-label: Getting started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Upload the data file via FTP (optional)

If you do not upload using drag-and-drop, you can upload customer attribute data via FTP to CX Enterprise.

You can upload the data after you create a customer attribute source and an FTP account in CX Enterprise. You create one FTP account per attribute source. The uploaded files are stored in the root folder of that account. The data must be in `.csv` format, with a second `.fin` file to indicate that the upload is complete. 

>[!IMPORTANT]
>
>Review [Customer attribute data files and sources](crs-data-file.md) before uploading the file. 

File uploads to the customer attributes FTP site can be done via FTP or SFTP: 

* You need a client that supports SFTP connections.
* You can connect with SFTP using either username/password or using no password, as described [here](https://experienceleague.adobe.com/docs/analytics/export/ftp-and-sftp/secure-file-transfer-protocol/ftp-sftp-cert-auth.html).

**To upload the data file via FTP** 

1. [Create a customer attribute source and upload the data file...](t-crs-usecase.md).

   Ensure that you are logged in to your FTP site at `ftp.adobe.com/<sftpname>`. 

1. Click **[!UICONTROL Actions]** > **[!UICONTROL File Upload]**.

1. Upload a `.fin` file, so that your file can be retrieved.

   The file type `.fin` is user-created and signals that the upload is finished. It can be a blank notepad file. For example, if you upload `crs123.csv`, you also upload `crs123.fin`. 

   If the upload is successful, both files are moved to a folder called **processed**. 

   See [Customer attribute data files and sources](crs-data-file.md) for important information about file names and structure.

## Set up an FTP account

Set up one FTP account per attribute source. 

On the [!UICONTROL File Upload and Schema Validation] page, click **[!UICONTROL FTP Setup]**.

![Edit a schema](assets/ftp-account.png)

The uploaded files are stored in the root folder of that account. The data must be in `.csv` format, with a second `.fin` file to indicate that the upload is complete.

The names you apply to strings, integers, and numbers are used to create [!DNL Analytics] metrics.

* **[!UICONTROL attribute:]** attribute data read from the uploaded `.csv` file.

* **[!UICONTROL Type:]** The data type, such as:

  * **String:** A sequence of characters.
    
  * **Integers:** Whole numbers.
  
  * **Numbers:** Can have up to two decimal places.
    
* **[!UICONTROL Display Name:]** A friendly name for the attribute. For example, you can change an attribute *customer age* to *customer Since*.

* **[!UICONTROL Description:]** A friendly description of the attribute.

