---
description: Learn how Adobe product and interface terms differ between CX Enterprise, Experience Cloud solutions, Creative Cloud, Experience League, and other support experiences.
solution: Experience Cloud
title: Terminology
feature-set: Experience Cloud Services
feature: Central Interface Components
topic: Administration
role: Admin
level: Experienced
exl-id: 3799f806-2794-43ab-9e70-06ee693871e7
TQID: 'https://experienceleague.adobe.com/mmk-by-ztmhgG6Mc76F4IDrjmXI5jqjIpwURHmbykVc'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: dab36b01-8bfa-48f3-8392-626455a058e6
    internal-label: Experience Cloud services
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id:
      id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
      internal-label: Support
    internal-label: ''
  - id:
      id: bdea9bc8-5600-45db-b85e-d74bb59dfcff
      internal-label: Organizations (AEC)
    internal-label: ''
  - id:
      id: fef08361-6ac5-460c-93fe-d063e40b6a49
      internal-label: Getting started
    internal-label: ''
role_v2:
  - id:
      id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
      internal-label: Admin
    internal-label: ''
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: d3cdead0-685a-4489-9250-4bb709942f66
    internal-label: Data collection
  - id: e9001ce2-5245-4a8e-8601-dd958009072f
    internal-label: Web experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
---
# Terminology

<!--
TQID: https://experienceleague.adobe.com/6wm7HcuAbaV1iV3AgN55dY5WR---BnMM7lJgN0HZDsk
-->

Use this table when the same word shows up in different Adobe experiences (CX Enterprise, marketing apps, design apps, or support sites). It is not a full glossary; see product-specific help on [Experience League](https://experienceleague.adobe.com) for deep definitions.

| Term | In CX Enterprise and this guide | Other common Adobe usage |
| --- | --- | --- |
| **Adobe CX Enterprise** | The unified web experience at `experience.adobe.com` where you open marketing applications, set preferences and notifications, and reach shared interface services (for example, Customer Attributes and [Audience Library](../services/audiences/overview.md)). Formerly *Adobe Experience Cloud*. | Not the same product as **Adobe Experience Platform** (customer data infrastructure, sandboxes, datasets). Not **Adobe Creative Cloud** (design and media apps). |
| **Adobe Experience Platform** | Appears when you connect data collection, identity, or platform agents to your solutions; some navigational search and AI features are Platform-backed. | A data and orchestration platform. Do not use "Experience Platform" when you mean the CX Enterprise shell or home page. |
| **Experience League** | Where Help and in-product links send you for **documentation**, **tutorials**, learning playlists, release notes, and community context for Adobe solutions. Start at [Experience League home](https://experienceleague.adobe.com). | Complements the **[Adobe Help Center](https://helpx.adobe.com/support.html)**, which emphasizes **account**, **plan**, **billing**, downloads, and cross-product troubleshooting for individuals and teams. Use Help Center for password resets, plan changes, and similar tasks; use Experience League for product how-to content. |
| **AI Assistant / agentic AI** | In-product assistants and orchestrated agents described in this guide's AI topics; access and credits depend on product entitlements. | Other Adobe surfaces (for example, **Firefly** or **Express**) use "AI" features with different scopes and policies. |
| **Organization** | Your **IMS organization**: the boundary for enterprise licensing, user directories, SSO, and Admin Console administration in CX Enterprise. See [Organizations and account linking](../administration/organizations.md). | Not an Analytics *report suite*, a Target *property*, or an Experience Platform *sandbox* (those are product-specific containers). |
| **Admin Console** | Enterprise control plane at `adminconsole.adobe.com` for users, product profiles, and identity; linked from CX Enterprise **Administration** topics. See [User and product management](../administration/admin-console.md). | Different from **in-product admin** inside each app (for example, Analytics admin tools or Journey Optimizer permissions screens). |
| **Product profile** | A license bundle in Admin Console that grants access to a product or capability; users must belong to a profile to be entitled. See [Manage products and profiles](https://helpx.adobe.com/enterprise/using/manage-products.html). | Not interchangeable with every in-product "workspace," "container," or "property" name; those vary by solution. |
| **Account linking** | Connecting an application login (for example, Analytics or Target credentials) to your Adobe ID for the organization so services recognize one user. See [Organizations and account linking](../administration/organizations.md). | Not the same as **directory sync**, **SSO**, or **federation** setup (those are org-wide identity decisions in Admin Console). |
| **Experience Cloud ID Service / ECID** | The persistent visitor identifier used across solutions; often deployed with tags or Web SDK. Still commonly referenced as **Experience Cloud ID** or **MID** in older Analytics discussions. See the [ID Service overview](https://experienceleague.adobe.com/docs/id-service/using/home.html). | Distinct from a single app's legacy cookie name or from **Experience Platform** identity graph concepts, though they can relate in an implementation. |
| **Customer Attributes** | CRM or enterprise attributes you upload and map for use in Analytics, Target, and related workflows via the People service. See the [Customer Attributes](../services/customer-attributes/attributes.md) topics. | Do not equate with **Audience Manager traits** alone or with every **Real-Time CDP** profile field without checking the product boundary. |
| **Audience Library** | CX Enterprise UI to compose and share audiences across integrated applications. | **Audience Manager** and **Target** also use "audiences," but segmentation rules and destinations differ by product. |
| **Segment** (Analytics) | A rule-based audience definition you can build in Adobe Analytics and, when supported, publish toward shared audiences. | In **Audience Manager**, segments combine **traits**; naming overlaps, but implementation is not identical. In **Target**, "audiences" replaced older "segment" labels in many places. |
| **Assets (Experience Cloud Assets)** | Shared folders and files for collaboration between CX Enterprise marketing workflows and approved **Creative Cloud** users. See [Assets overview](../services/assets/experience-cloud-assets.md). | In **Creative Cloud**, "assets" usually means design files (PSD, AI, INDD). Same word, different sharing and governance model. |

{style="table-layout:auto"}

