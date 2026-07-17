---
title: '[!DNL Customer Attributes] Support for California Consumer Privacy Act'
description: Learn about [!DNL Customer Attributes] support for California Consumer Privacy Act
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 320defc7-2cd5-4481-955d-77cf6fbfef6d
TQID: 'https://experienceleague.adobe.com/YPl1rlZRciwN6GM7mtkqMKjPsW-H1ueMG4zqbH8auho'
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
---
# [!DNL Customer Attributes] support for California Consumer Privacy Act

This page describes [!DNL Customer Attributes] support for the California Consumer Privacy Act (CCPA).

>[!IMPORTANT]
>
>The contents of this document are not legal advice and are not meant to substitute for legal advice. Consult with your legal counsel for advice concerning the (CCPA).

The CCPA is California's new privacy law, which is effective January 1, 2020. CCPA provides California residents new rights regarding their personal information and imposes data protection responsibilities on certain entities who conduct business in California. CCPA provides consumers with the right to access and delete their personal information and the right to opt out of certain activities that qualify as "selling" personal information to a third party.

As a business, you determine the personal data that Adobe CX Enterprise processes and stores on your behalf.

As your service provider, Adobe CX Enterprise provides support for your business to fulfill its obligations under CCPA that are applicable to the use of CX Enterprise products and services. This support includes managing requests to access and delete personal information.

This document describes how [!DNL Customer Attributes] supports your data subjects' CCPA data access and deletion rights using the Adobe Experience Platform Privacy Service API and Privacy Service UI.

For more information about the Adobe Privacy services for CCPA, see the [Adobe Privacy Center](https://www.adobe.com/privacy/ccpa.html).

## Required setup to send requests for [!DNL Customer Attributes]

To make requests to access and delete data for [!DNL Customer Attributes], you must:

1. Identify the following:

   * [Organization ID](../../administration/organizations.md)
   * Alias ID of CRS Data Source you want to act on
   * CRM ID of the profile you want to act on

    Your organization ID is a 24-character alphanumeric string appended with @AdobeOrg. You need the organization's ID to submit requests to the Privacy API. Contact Adobe Customer Care at `gdprsupport@adobe.com` if you cannot locate the ID.

1. In [!UICONTROL Privacy Service], you can submit Access and Delete requests to Customer Attributes, and check the status of existing requests.

## Required field values in [!DNL Customer Attributes] JSON Requests

"company context": 

* "namespace": **imsOrgID**
* "value": <*your organization ID value*>

"users": 

* "key": <*usually the name of the customer*> 
* "action": either **access** or **delete**
* "user IDs":
    * "namespace": <*Alias ID of CRS Data Source*>
    * "type": **integrationCode**
    * "value": <*CRM ID*>
* "include": **CRS** (which is the Adobe product that applies to the request)
* "regulation": **ccpa** (which is the privacy regulation that applies to the request)

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

## Data fields returned for access requests

```json
attributes:
{
"value": "<*value*>",
"key": "<*key*>",
"displayName": "<*displayName*>"
}
```
