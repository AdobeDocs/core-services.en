---
description: Learn the considerations and best practices regarding personally identifiable information (PII) uploaded and used in CX Enterprise.
solution: Experience Cloud
title: Privacy Considerations for [!DNL Customer Attributes]
feature: Customer Attributes
topic: Administration
role: Admin
level: Experienced
exl-id: 27c026ff-198b-4f49-9718-f25f77a9e716
TQID: https://experienceleague.adobe.com/4L-qz0n3h97DduJvPGGoJPl1VvrPAKJTeUnkJGs6xvc
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
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
---
# Privacy considerations for [!DNL Customer Attributes]

Considerations and best practices regarding personally identifiable information (PII) uploaded and used in Adobe CX Enterprise.

* First and last name
* Home or other physical address
* Email address
* Telephone number
* Social Security Number
* Other identifier that permits physical or online contacting of an individual. (Varies by location. Please verify and comply with local laws and regulations related to privacy and PII for all the places where you do business.)

Adobe provides tools that allow advertisers to collect behavioral information about consumers that visit their sites or use their applications. Adobe also provides tools allow advertisers to enhance this information with offline or external customer records that the advertiser may have within other information management systems. 

One common reason advertisers do this is to improve the information available when making consumer-appropriate marketing and advertising decisions. Adobe Analytics and Target allow advertisers to upload personally identifiable information (PII), such as email addresses, only after it has been hashed to make it impossible to use for contacting the individual. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe, such as medical records, financial account information, and information about minors. 

Adobe realizes that these types of marketing and advertising decisions may have consumer privacy implications, which is why Adobe has built in privacy controls to help advertisers meet their consumers' expectations. Adobe recommends that its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. 

## Best practices

When uploading PII to Adobe Analytics or Adobe Target, Adobe recommends that the customer hashes PII prior to uploading it to Adobe. Hashed information can still be used for analysis and for marketing purposes. As a reminder, Adobe prohibits advertisers from sending sensitive personal information to Adobe Analytics and Adobe Target, such as medical records, financial account information, and information about minors. 

Adobe recommends that its advertisers carefully consider which information is appropriate to use for marketing purposes and in which circumstances the advertiser has permission to use such information. 

As consumer privacy law remains in flux, Adobe recommends that advertisers respect three common tenets: 

1. Do what you say (in your privacy policy).
1. Say what you do (in your privacy policy).
1. Do not surprise your consumers.

With these expectations in mind, Adobe recommends that when an advertiser associates browsing activities to PII, the advertiser provides notices or personalization indicating that the consumer is authenticated. An example of this is including a greeting within the header of the website. Adobe also recommends that advertisers describe in its privacy policy what type of browsing information it associates with PII and under what circumstances browsing information is associated with PII. Lastly, Adobe strongly recommends advertisers review the opt-out choices they provide their consumers to understand whether and how they can use unauthenticated profile information post opt-out.
