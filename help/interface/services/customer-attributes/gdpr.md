---
title: '[!DNL Customer Attributes] Support for General Data Protection Regulation'
description: Learn about Customer Attributes support for General Data Protection Regulation
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 02417c0c-6780-4699-9470-f1685c3cd25d
TQID: 'https://experienceleague.adobe.com/eKqqNOKxc2QE4mAzsp1y6FT724ccJDtpmA1ydYLD0Fk'
product_v2:
  - id: e1971122-7081-4556-9222-8a31bd71800c
    internal-label: Experience Cloud Services
role_v2:
  - id:
      id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
      internal-label: Admin
    internal-label: ''
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
---
# [!DNL Customer Attributes] support for General Data Protection Regulation

This page describes how [!DNL Customer Attributes] supports General Data Protection Regulation (GDPR).

>[!IMPORTANT]
>
>The contents of this document are not legal advice or meant to substitute for legal advice. Consult with your legal counsel for advice concerning GDPR.

The [General Data Protection Regulation](https://business.adobe.com/privacy/general-data-protection-regulation.html), a law in effect May 25, 2018, gives all individuals (data subjects) within the borders of the European Union (EU) control of their personal data. It also simplifies the regulatory environment for international business. This law applies to all businesses (data controllers) that offer goods or services to, monitor the behavior of, or collect personal data from individuals within the borders of the EU at the time their personal data is processed, regardless of the data controller's business location.

Adobe CX Enterprise acts as a data processor for any personal data it receives and stores on behalf of its customers. As a data controller, you determine the personal data that Adobe CX Enterprise processes and stores on your behalf.

This document describes how [!DNL Customer Attributes] supports your data subjects' GDPR data access and deletion rights using the Adobe Experience Platform Privacy Service API and Privacy Service UI.

For more information about what GDPR means for your business, see [GDPR and Your Business](https://business.adobe.com/privacy/general-data-protection-regulation.html).

## Required setup to send requests for [!DNL Customer Attributes]

To make requests to access and delete data for [!DNL Customer Attributes], you must:

1. Identify the following:

   * [Organization ID](../../administration/organizations.md)
   * Alias ID of CRS Data Source you want to act on
   * CRM ID of the profile you want to act on

   Your [organization ID](../../administration/organizations.md) is a 24-character alphanumeric string appended with @AdobeOrg. You need the organization's ID to submit requests to the Privacy API. Contact Adobe Customer Care at `gdprsupport@adobe.com` if you cannot locate the ID.

1. In [!UICONTROL Privacy Service], you can submit Access and Delete requests to [!DNL Customer Attributes], and check the status of existing requests.

## Required field values in [!DNL Customer Attributes] JSON requests

"company context":

* "namespace": **imsOrgID**
* "value": <*your IMS Org ID value*>

"users":

* "key": <*usually the name of the customer*>
* "action": either **access** or **delete**
* "user IDs":
    * "namespace": <*Alias ID of CRS Data Source*>
    * "type": **integrationCode**
    * "value": <*CRM ID*>
* "include": **CRS** (which is the Adobe product that applies to the request)
* "regulation": **gdpr** (which is the privacy regulation that applies to the request)

## Example of JSON request

```json
{
  "companyContexts": [
    {
      "namespace": "imsOrgID",
      "value": "<IMS_ORG_ID>"
    }
  ],
  "users": [
    {
      "key": "<KEY>",
      "action": [
        "<access/delete>"
      ],
      "userIDs": [
        {
          "namespace": "<Alias ID of CRS Data Source>",
          "type": "integrationCode",
          "value": "<CRM ID>"
        }
      ]
    }
  ],
  "regulation": "<gdpr/ccpa/pdpa>",
  "include": [
    "CRS"
  ]
}
```

## Data Fields returned for access requests

```json
attributes:
{
"value": "<*value*>",
"key": "<*key*>",
"displayName": "<*displayName*>"
}
```
