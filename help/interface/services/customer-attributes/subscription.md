---
description: Learn about solution data sources and configuring subscriptions. Subscriptions enable the customer attribute data flow between Experience Cloud and applications (Analytics and Target).
solution: Experience Cloud
title: How to configure subscriptions 
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: cfa2aa5c-337f-401e-80eb-cbe36cb1d41e
---
# How to configure subscriptions in Experience Cloud

Learn about application data sources and configuring subscriptions. Subscriptions enable the [!DNL customer attribute] data flow between Experience Cloud and applications ([!DNL Analytics] and [!DNL Target]).

For example, an Adobe Analytics subscription enables attribute data in reports. If you use Adobe Target, you can upload customer attributes for targeting and segmentation. 

**[!UICONTROL customer attribute Source]** > **[!UICONTROL Create New customer attribute Source]** > **[!UICONTROL New]** 

![Configure subscriptions in Experience Cloud](assets/configure_subscription_page.png) 

| Element | Description |
|--- |--- |
|Solution|**Adobe Analytics**<br>Select [!DNL Analytics], specify the report suites to that you want to receive attribute data, and the attributes to include.<br>**Adobe Target**<br>You can upload customer attributes for targeting and segmentation. This feature is useful if want to target a test based on attribute data, or make the data available for segmentation in Analytics.<br>Uploaded customer attribute data for a visitor is available at login, in **[!DNL Target]** > **Audiences**.<br>Multiple data sources are supported. When you set customer IDs on your website, verify that at least one of the aliases is subscribed to [!DNL Target].|
|Report Suite (Adobe Analytics)|The report suites from Analytics.<br>You cannot add more than a total of 10 report suites to the Analytics subscriptions within a single attribute source. When choosing which report suites to include, consider the following suggestions:<ul><li>Choose report suites that have a common set of authenticated customers. If the authenticated customers in one report suite do not overlap with the authenticated customers in another report suite, separate these report suites into different attribute sources.</li><li>If possible, the report suites included in an attribute source should have similar traffic volume.</li></ul><br>If you have more than 10 report suites that have a common set of authenticated customers, you can configure additional customer attribute sources, each with up to 10 report suites.|
|attributes to Include (Analytics and [!DNL Target])|The attributes that you want to send to the application. <br>When configuring subscriptions and selecting attributes, the following limits apply _per report suite,_ depending on the applications you own:<ul><li>Foundation: 0</li><li>Select: 3</li><li>Prime: 15</li><li>Ultimate: 200</li><li>Standard: 3 total</li><li>Premium: 200 per report suite</li><li>[!DNL Target] Standard: 5</li><li>[!DNL Target] Premium: 200</li></ul><br>**Note:** When you upgrade to Analytics Premium, there is a 24-hour delay before additional attributes are available. You may see an attribute Subscription Max error issued during this delay.|

{style="table-layout:auto"}
