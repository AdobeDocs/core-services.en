---
title: Adobe Experience Platform Web SDK Cookies
description: Learn how the Web SDK uses cookies applicable to your implementation.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
TQID: https://experienceleague.adobe.com/jysQ5m7o0cI3ECKz2RWZB4Kt3own7XAPm04pr4yLh-k
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
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Adobe Experience Platform Web SDK cookies

The Adobe Experience Platform Web SDK uses cookies to store values specific to your implementation.

| Name | Max age | Size | Description |
| --- | --- | --- | --- |
| **`AMCV_###@AdobeOrg`** | 34128000 (395 days) | 100-120 bytes (variable) | Present when [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/idmigrationenabled) is enabled. It helps when transitioning to the Web SDK while some parts of the site still use `visitor.js`. The Web SDK both reads and writes to this cookie during migration. |
| **`com.adobe.alloy.getTld`** | None (immediately deleted) | N/A | Temporary helper cookie used internally by the Web SDK to determine the top-level domain of the current site. Once the top-level domain is established, the cookie is deleted. It does not store behavioral or profile data. |
| **`demdex`** | 15552000 (180 days) | varies | Present if Audience Manager ID synchronization is enabled. Audience Manager sets this cookie to assign a unique ID and support ID sync, segmentation, modeling, and reporting. See `demdex` in [Audience Manager cookies](audience-manager.md). |
| **`kndctr_<orgId>_identity`** | 34128000 (395 days) | 100-120 bytes (variable) | Stores the ECID and other related information for that device. |
| **`kndctr_<orgId>_cluster`** | 1800 (30 minutes) | 3-5 bytes | Stores the Edge Network region (location hint) that serves the current user's requests. The region is used in the URL path so that the Edge Network can route the request to the correct region. If a user connects with a different IP address within the cookie lifetime, the request is again routed to the closest region. |
| **`kndctr_<orgId>_consent`** | 15552000 (180 days) | 10-11 bytes | Stores the visitor's consent preferences. Always set regardless of consent because it stores the consent preferences itself. |
| **`kndctr_<orgId>_consent_check`** | 7200 (2 hours) | | Session-scoped helper that signals the Edge Network to re-check consent server-side after the TTL expires. It enforces a TTL on cached consent. |
| **`kndctr_<orgId>_personalization`** | 34128000 (395 days) | | Stores session information that Adobe Target uses to personalize content. |
| **`mbox`** | 63072000 (2 years) | | Present when [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) is enabled. It allows the Target [mbox cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) to be set by the Web SDK. |
| **`mboxEdgeCluster`** | 1800 (30 minutes) | | Present when [`targetMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/collection/js/commands/configure/targetmigrationenabled) is enabled. It allows the Web SDK to communicate the correct edge cluster to `at.js` so that Target profiles can stay in sync as users navigate across a site. |
| **`s_ecid`** | 63115200 (2 years) | ~45 bytes | Contains a copy of the Experience Cloud ID (ECID/MID) in the format `s_ecid=MCMID\|<ECID>`. Acts as a first-party backup of the ECID, primarily for CNAME (first-party) scenarios. |

The Edge Network sets all cookies with the `secure` and `sameSite="none"` attributes. If you currently have both secure and non-secure sections on your website, user identification can be inaccurate. When a user navigates from a secure section of the site to a non-secure section, the Edge Network generates a new `ECID` with the request.
