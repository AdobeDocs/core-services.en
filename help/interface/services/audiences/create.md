---
title: How to Create an Audience in Audience Library
description: Find out how to use attribute rules to create a sharable  audience in Audience Library. Learn to configure a rule and define a composite audience.
solution: Experience Cloud
uuid: 7e622539-296e-4ff3-93b0-ec1c08b35429
feature: Audience Library
topic: Administration
role: Admin
level: Experienced
exl-id: b65a12f5-fa89-400a-b279-13c381cd6c22
TQID: https://experienceleague.adobe.com/xXhiBeGGEVpvdjZdpL2Q9-3eDn-gN58dynb56daQcig
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
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create an audience

In [!UICONTROL Audience Library], you can use attribute rules to create an audience and define a composite audience for sharing in CX Enterprise applications.

This article helps you understand how to:

* Create an audience
* Create a rule
* Use rules to define a composite audience

The following graphic represents two rules in a composite audience.

![Two rules in a composite audience](assets/audience_sharing.png)

Each circle represents a rule that defines audience membership. Visitors that qualify as members in both audience rules overlap to become the composite, defined audience.

>[!NOTE]
>
>The audience is fully defined after data collection for the specified period completes.

The following example shows how to create the rules for a composite audience. This audience is composed of:

* Home & Garden section derived from page data, or raw analytics data.
* Chrome and Safari users derived from an [!DNL Adobe Analytics] segment [published](overview.md) to [!DNL CX Enterprise].

  ![Create the rules for a composite audience](assets/audience_create.png) 

**To create an audience**

1. Click [!DNL CX Enterprise] apps (![Apps icon](assets/apps-icon.png)), then click **[!UICONTROL People]** > **[!UICONTROL Audience Library].**

1. On the [!UICONTROL Audiences] page, click **[!UICONTROL New]**. ![New audience](assets/add_icon_small.png)

   ![Create an audience](assets/audience_create_new.png)

1. On the [!UICONTROL Create New Audience] page, complete the **[!UICONTROL Title]** and **[!UICONTROL Description]** fields.
1. Under [!UICONTROL Rules], select a reference report suite, then an attribute source:

   * **[!UICONTROL Real-Time Analytics Data:]** (or Raw data) This is attribute data derived from Real-Time Analytics image requests. It includes eVars and events. You must select a report suite when using this attribute source, and define the dimension or event to include. This report suite selection provides the variable structure used by the report suite.
   
      >[!NOTE]
      >
      >Due to caching, deleted report suites in Analytics require 12 hours before the deletion is shown in CX Enterprise.

   * **[!UICONTROL CX Enterprise:]** attribute data derived from [!DNL CX Enterprise] sources. For example, this can be data from audience segments you create in [!DNL Analytics], or data from [!DNL Audience Manager].

1. Define audience rules, then click **[!UICONTROL Save].**

**Example: Define rules for composite audience**

>[!NOTE]
>
>You should have an understanding of your implementation variables when defining audience rules.

Under [!UICONTROL Rules], define the *`Home & Garden`* attribute selections:

* **[!UICONTROL Attribute Source:]** Raw Analytics Data
* **[!UICONTROL Report Suite:]** Report Suite 31
* Dimension = **[!UICONTROL Store (Merch) (v6)]** > **[!UICONTROL Equals]** > **[!UICONTROL Home & Garden]**

![Attribute selections in Audience Library](assets/home_garden.png)

The *Chrome & Safari Visitors* is an audience segment shared from Analytics:

* **[!UICONTROL Attribute Source:]** CX Enterprise
* **[!UICONTROL Dimension:]** Chrome & Safari Visitors

![Chrome & Safari Visitors](assets/chrome_safari.png)

For comparison, you might add an *OR* rule to see all visitors to a site section, such as Patio & Furniture.

![OR rule for an audience](assets/audiences_rule_patio.png)

The resulting rule is a defined audience comprising Chrome & Safari users who visited Home & Garden. The Patio & Furniture segment provides additional insight into all visitors visiting that site section.

![Defined audience in CX Enterprise](assets/defined_audience.png)

* **Historical Estimate:** (Dotted circle) Represents rules created based on [!DNL Analytics] data.
* **Actual Audience:** (Solid circle) Any rule created that has 30 days of data from Audience Manager. When the Audience Manager data reaches 30 days, the line becomes solid and represents actual numbers.

After the data collection completes for the specified period, the circles combine to show a defined audience.

After the audience is saved, it is available for other CX Enterprise applications. For example, you can include a shared audience in an Adobe Target [activity](https://experienceleague.adobe.com/en/docs/target/using/activities/activities).
