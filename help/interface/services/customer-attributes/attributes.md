---
title: "[!DNL Customer attributes]"
description: Learn about [!DNL customer attributes] in Experience Cloud. Discover how to upload customer attribute data for use in Adobe Analytics and Adobe Target.
solution: Experience Cloud,Target,Analytics
feature: Customer Attributes
role: Admin
topic: Administration
level: Experienced
exl-id: fe8ad013-76da-49f8-aa51-dc5f6c1b1d79
---
# [!DNL Customer attributes] in Experience Cloud

[!DNL Customer attributes] in Experience Cloud enables you to upload your captured enterprise data from a customer relationship management (CRM) database. You can upload the data into a customer attribute data source in Experience Cloud, then use the data in [!DNL Adobe Analytics] and [!DNL Adobe Target].  

## Locate the [!DNL customer attributes] feature

1. Log in to the [!DNL Experience Cloud] and select the Menu ![menu](assets/menu-icon.png) icon.

1. Select **[!UICONTROL Customer Attributes]**.

![Customer attributes overview](assets/custom_reports.png)

## Prerequisites for uploading [!DNL customer attributes] {#prerequisites}

* **Group membership:** To upload customer attribute data, users must be members of the Customer Attributes group. You must also belong to either an Adobe Analytics group or an Adobe Target group.

  To know whether your company has access to customer attributes, your [!DNL Experience Cloud] administrator should log into the [Experience Cloud](https://experience.adobe.com). Navigate to **[!UICONTROL Admin Console]** > **[!UICONTROL Products]**. If *[!DNL Customer Attributes]* displays as one of the [!UICONTROL product profiles], you are ready to begin.

  Users that are added to [!DNL Customer Attributes] see the [!UICONTROL Customer Attributes] menu item on the left side of the Experience Cloud interface.

* **Adobe Target** `at.js` (any version) or `mbox.js` version 58 or later is required for customer attributes.

  See [How to deploy at.js](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/overview.html).

## What is enterprise customer data? {#enterprise_data}

Enterprise data resides in other systems. It can be complex and mean different things to different people. This data can include information such as memberships, loyalty level, age, gender, products owned, interests, and Lifetime Value.

The following image is an example of a data file showing subscriber data for products, including member IDs, entitled products, most-launched products, and so on.

![What is enterprise customer data?](assets/01_crs_usecase.png)

After you create the data file, you can upload it to the customer attribute source that you create in **[!UICONTROL Experience Cloud]** > **[!UICONTROL Customer attributes]**.

See [Upload customer attribute data](t-crs-usecase.md) to learn this workflow.

## Examples of customer attributes in Analytics and Target {#examples}

After the data resides in Experience Cloud, you can customize it and share it to solutions for reporting, segmentation, activities, and campaigns.

For example:

| Solution | Advantages and Use Cases |
|--- |--- |
|Adobe Analytics|Marketers and analysts can understand:<ul><li>The online campaigns that are most effective with your gold-level customers.</li><li>The products that gold-level customers search for versus products that platinum-level customers search for.</li><li>Whether your site redesign is having a positive impact on conversion rates for older customers.</li><li>The products that customers with a low lifetime value tend to research on my site.</li></ul>|
|Adobe Target|Attribute data enables Adobe Target users to:<ul><li>Show loyalty club members special discounts and offers.</li><li>Recommend more expensive products to your luxury customers.</li><li>For customers who already receive emails, show an up-sell offer in the space normally reserved for email sign-ups</li></ul>|

{style="table-layout:auto"}
