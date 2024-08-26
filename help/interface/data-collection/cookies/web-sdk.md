---
title: Adobe Experience Platform Web SDK Cookies
description: Learn how the Web SDK uses cookies applicable to your implementation.
solution: Experience Cloud
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 14f06dc9-255e-4a6c-adec-471107cf202e
---
# Adobe Experience Platform Web SDK cookies

The Adobe Experience Platform Web SDK uses cookies to store values specific to your implementation.

| Name | Max age | Description |
|---|---|---|
| **kndct_orgid_identity** | 34128000 (395 days) | Stores the ECID, as well as other information related to the ECID. |
| **kndctr_orgid_consent_check** | 7200 (2 hours) | Signals the server to look up the consent preferences server side. |
| **kndctr_orgid_consent** | 15552000 (180 days) | Stores the user's consent preference for the website. |
| **kndctr_orgid_cluster** | 1800 (30 minutes) | Stores the Edge Network region that serves the current user's requests. The region is used in the URL path so that the Edge Network can route the request to the correct region. If a user connects with a different IP address or in a different session, the request is again routed to the closest region. |
| **mbox** | 63072000 (2 years) | Present when the Target migration setting is set to true. It allows the Target [mbox cookie](https://developer.adobe.com/target/implement/client-side/atjs/atjs-cookies/) to be set by the Web SDK. |
| **mboxEdgeCluster** | 1800 (30 minutes) | Present when the Target migration setting is set to true. It allows the Web SDK to communicate the correct edge cluster to `at.js` so that Target profiles can stay in sync as users navigate across a site. |
| **AMCV_###@AdobeOrg** | 34128000 (395 days) | Present when [`idMigrationEnabled`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/idmigrationenabled) is enabled. It helps when transitioning to Web SDK while some parts of the site are still using `visitor.js`. |

The Edge Network sets all cookies with the `secure` and `sameSite="none"` attributes. If you currently have both secure and non-secure sections on your website, user identification can be inaccurate. When a user navigates from a secure section of the site to a non-secure section, the Edge Network generates a new `ECID` with the request.
