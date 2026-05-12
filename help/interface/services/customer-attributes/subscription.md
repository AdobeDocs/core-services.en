---
description: Learn how to configure subscriptions in [!DNL Customer Attributes] for Analytics and Target, and to activate a data source.
solution: Experience Cloud
title: How to Configure Subscriptions in [!DNL Customer Attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
TQID: https://experienceleague.adobe.com/I--LZ-Nqu0VdVAAs8qvv88pZTcaRQ97XiHWXd15WQcE
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
# Configure customer attribute subscriptions

[!DNL Customer Attributes] subscriptions enable the customer attribute data flow between CX Enterprise and applications ([!DNL Analytics] and [!DNL Target]).

For example, an Adobe Analytics subscription enables attribute data in reports. If you use [!DNL Adobe Target], you can upload customer attributes for targeting and segmentation. 

**To configure subscriptions and activate the data source**

1. Locate your data source in [!DNL Customer Attributes] for edit:

    In [!DNL CX Enterprise], click **[!UICONTROL Apps]** ![menu](assets/menu-icon.png) > **[!DNL Customer Attributes]**.

1. On [!UICONTROL Edit Customer Attribute Source], click **[!UICONTROL File Upload]**. 

1. Click **[!UICONTROL Configure Subscriptions]**. 

    ![Configure subscriptions in CX Enterprise](assets/configure-subscriptions.png) 

1. To activate the customer attribute source, click **[!UICONTROL Active]**, then click **[!UICONTROL Save]**.

1. To configure a subscription to [!DNL Analytics] or [!DNL Target], click **[!UICONTROL Configure]**.

    The following example shows a [!DNL Target] subscription:

   ![Step Result](assets/subscription-target.png)

    | Element | Description |
    | --- | --- |
    |Solution|**Adobe Analytics**<br>Select [!DNL Analytics], specify the report suites to that you want to receive attribute data, and the attributes to include.<br>**Adobe Target**<br>You can upload customer attributes for targeting and segmentation. This feature is useful if want to target a test based on attribute data, or make the data available for segmentation in Analytics.<br>Uploaded customer attribute data for a visitor is available at sign in, in **[!DNL Target]** > **Audiences**.<br>Multiple data sources are supported. When you set customer IDs on your website, verify that at least one of the aliases is subscribed to [!DNL Target].|
    |Report Suite (Adobe Analytics)|The report suites from Analytics.<br>You cannot add more than a total of 10 report suites to the Analytics subscriptions within a single attribute source. When choosing which report suites to include, consider the following suggestions:<ul><li>Choose report suites that have a common set of authenticated customers. If the authenticated customers in one report suite do not overlap with the authenticated customers in another report suite, separate these report suites into different attribute sources.</li><li>If possible, the report suites included in an attribute source should have similar traffic volume.</li></ul><br>If you have more than 10 report suites that have a common set of authenticated customers, you can configure additional customer attribute sources, each with up to 10 report suites.|
    |Attributes to Include (Analytics and [!DNL Target])|The attributes that you want to send to the application. <br>When configuring subscriptions and selecting attributes, the following limits apply _per report suite,_ depending on the applications you own:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 total</li><li>Premium: 200 per report suite</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Note:** When you upgrade to Analytics Premium, there is a 24-hour delay before additional attributes are available. You may see an attribute Subscription Max error issued during this delay.|

1. Click **[!UICONTROL Save]**.
