---
description: Get answers to frequently asked questions about [!DNL Customer Attributes] in Adobe CX Enterprise, for Adobe Analytics and Adobe Target.
solution: Experience Cloud
title: Frequently Asked Questions about [!DNL Customer Attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 6031e544-822b-4843-b3d8-98a36a3c40e8
TQID: https://experienceleague.adobe.com/ZAKogDXCbaZHOiyzlgg6Od0pxGwWi2w9yXtPnKWZKUw
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: Experience Cloud
feature_v2:
  - id: fc7979f3-56c3-43ca-9784-f1ea3dc69c4b
    internal-label: Integrations
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
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c4147b6e-073b-4d3c-9ab1-d60f2f4434ef
    internal-label: Behavioral data
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: fd2e3797-f2ea-4b36-a9af-52acf5e90513
    internal-label: Customer profiles
---
# Frequently asked questions about [!DNL Customer Attributes]

Frequently asked questions and best practices for [!DNL Customer Attributes] in Adobe Analytics and Adobe Target.

## Best practices and limitations 

Guidance and limitations when using [!DNL Customer Attributes].

| Issue | Description |
| --- | --- |
|[!DNL Customer Attributes] [subscription](subscription.md) limitations|When you upgrade to Analytics Premium, there is a 24-hour delay before more attributes are available. You might see an [!UICONTROL attribute Subscription Max] error issued during this delay.|
|Multiple logins on the same device|When using [!DNL Customer Attributes] to upload customer profiles into a data source, Adobe recommends against users sharing devices (meaning, the same CX Enterprise ID). The CX Enterprise ID (ECID) persists on the device. Sharing devices can cause the ECID to link multiple users to the same ECID, causing unexpected results in [!DNL Target]. **Note:** For Mobile, the ECID is permanent after the Mobile app is installed. Reinstall the app to generate a new ECID. For Web, a new ECID is generated after the browser cookie is cleared.|
|Daily frequency upload limitation| Adobe recommends that you update [!DNL Customer Attributes] only once per day. You must wait at least 24 hours to upload another customer profile data file for the same set of profiles.|
|Custom Analytics ID (`s.visitorID`)|Setting a customer ID using `s.visitorID` is a method of identifying users in Adobe Analytics. However, integrations in which [!DNL Analytics] data is exported or imported using the ID Service do not function when a visitor is identified using `s.visitorID.`<br>This includes, but is not limited to, shared Audiences, [!DNL Analytics] for Adobe Target (A4T), and [!DNL Customer Attributes].<br>For these integrations, setting a custom Analytics ID is not supported.|
|Character length limitations in [!DNL Analytics]|When creating an [!DNL Analytics] [subscription](subscription.md), field lengths for the uploaded files are truncated to 255.|

{style="table-layout:auto"}

## FAQ about [!DNL Customer Attributes] 

| Question | Answer |
| --- | --- |
|Can I receive notifications about upload status for [!DNL Customer Attributes]?|Yes.|
|What should I do to get started with [!DNL Customer Attributes]?|<ol><li>Get provisioned. If you are an Adobe Analytics customer, Adobe is provisioning you for [!DNL Customer Attributes]. If you use only Adobe Target and do not have Analytics, request provisioning for core services by contacting customer Care.</li> <li>Have a conversation with your CRM team. Find out what kind of customer data is available that you want to use in Analytics and throughout CX Enterprise.</li><li>Implement core services.</li></ol> See [prerequisites](t-crs-usecase.md#prerequisites-for-using-customer-attributes) before uploading data to learn about enabling users to use this feature.|
|How many customer attributes am I allowed to use?|You can upload hundreds of `.csv` columns to the customer attribute service. However, when configuring subscriptions and selecting attributes, the following limits apply (per report suite), depending on the applications you own:  <ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 total</li><li>Premium: 200</li><li>Adobe Target Standard: 5</li><li>Adobe Target Premium: 200</li></ul>|
|Is migrating to the CX Enterprise ID Service required?|Migration depends on the applications you use. <ul><li>Adobe Analytics: Strongly recommended </li><li>Adobe Target: Required. </li></ul>Using the CX Enterprise ID service enables the latest CX Enterprise functionality, including real-time audiences, the Adobe Target modernization, Analytics integration, and video heartbeat tracking. |
|How does the customer attribute functionality relate to Adobe Audience Manager?|While Audience Manager can receive data to perform audience identification, it cannot perform analytics functionality that ties attributes to historical behavioral data. It also does not provide the reporting, analysis, and segmentation capabilities that are available in Adobe Analytics. [!DNL Customer Attributes] enables rich data from across applications to be tied together and associated with a single ID for use across CX Enterprise. <br>In Adobe Target, customer attributes appear as individual attributes that can be combined with other rules to build audiences. Audiences shared to the [!UICONTROL People] service are full audiences that cannot be modified.|
|**(Adobe Analytics only)** How is this functionality different from what is provided in Analytics premium?|In the past, customers interested in combining customer attribute data with Analytics data have relied heavily on the Data Workbench tool for this functionality. [!DNL Customer Attributes] exposes this functionality to a wider audience by providing customer attributes as dimensions and metrics in Report Builder. Analytics Standard customers have access to [!DNL Customer Attributes], but with limited capabilities. The full capability is available to Analytics Premium customers.|
|**(Adobe Target Only)** Can I pre-load or upload data for customers that Adobe Target has never seen?|Yes. When the visitor makes their first request to Adobe Target, the system fetches the existing information Adobe has about them from [!DNL Customer Attributes] and use that data for targeting. **Note:**  Retrieving this data can take up to 20 min from the visitor's first interaction with Adobe Target.|
|**(Adobe Target Only)** Can I create a super audience by combining customer attribute data with shared audience data?|No. Shared audience data is a completed audience.|
|**(Adobe Target only)** How does [!DNL Customer Attributes] compare to Adobe Target's bulk profile API?|The bulk profile API enables Adobe Target profiles to be updated directly via the API, either for an individual profile or in bulk. The capability is similar to [!DNL Customer Attributes], with the following key differences:<ul><li>The profile API is a REST API call and [!DNL Customer Attributes] uses FTP.</li><li>Adobe Target's profile API only sends data to Adobe Target instead of to the whole CX Enterprise.</li><li>[!DNL Customer Attributes] provides a simple interface to create and manage this external data.</li></ul>|
|**(Adobe Target only)** Does uploading data from [!DNL Customer Attributes] to Adobe Target extend the Adobe Target visitor's profile lifetime?|Yes. See [Visitor Profile Lifetime](https://experienceleague.adobe.com/docs/target/using/audiences/visitor-profiles/visitor-profile.html) in Adobe Target Help.|
|**(Adobe Target only)** Can I target on the data uploaded in [!DNL Customer Attributes] immediately after the visitor is identified by the customer ID?|Yes. On the server call to Adobe Target, which includes the mbox third-party ID, all customer attribute data are available.|
|**(Adobe Target only)** What does the **[!UICONTROL Sync Status]** column represent for files uploaded in customer attribute source?|The number of records published and synced by Adobe Target can be viewed by selecting the Sync Status icon against a specific attribute file. `Sync %` is a real-time metric that specifies the % of profiles that have been synced in Adobe Target.<br> **Note:** It may take up to 24 hours for attributes to sync with Adobe Target.|
|What do the file upload metrics represent in [!DNL Customer Attributes] Source?|You can check the status of attributes uploaded to [!DNL Customer Attributes] with the help of following metrics: <ul><li>Records:  Number of records in the attributes file.</li><li>**New Records:** Number of new records present in the attributes file.</li> <li>**Updated Records:** Number of records in that exist in [!DNL Customer Attributes] with updated values in the file.</li><li>**All Data (Records):** Total number of records successfully uploaded to [!DNL Customer Attributes].</li></ul>|

{style="table-layout:auto"}
