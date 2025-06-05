---
description: Learn how to upload customer attribute data via FTP to Experience Cloud.
solution: Experience Cloud
title: Upload the customer attribute Data File via FTP 
feature: Customer attributes
topic: Administration
role: Admin
level: Experienced
exl-id: ed9e4a8f-493a-4a0f-a87e-674c7da95b99
---
# Optional - Upload the data file via FTP

If you do not upload using drag-and-drop, you can upload customer attribute data via FTP to Experience Cloud.

You can upload the data after you create a customer attribute source and an FTP account in Experience Cloud. You create one FTP account per attribute source. The uploaded files are stored in the root folder of that account. The data must be in `.csv` format, with a second `.fin` file to indicate that the upload is complete. 

>[!IMPORTANT]
>
>Review [Data file requirements for uploading customer attributes](crs-data-file.md) before uploading the file. 

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

   See [Data file requirements for uploading customer attributes](crs-data-file.md) for important information about file names and structure.
