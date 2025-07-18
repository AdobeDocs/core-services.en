---
description: Learn about Adobe Analytics cookies in Adobe Experience Cloud.
solution: Analytics
title: Adobe Analytics Cookies 
uuid: e2d3d61d-2708-48b2-a7e6-2331f2aed8e0
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bc8ce894-f98c-4475-8a07-d74ae76f7451
---
# Adobe Analytics cookies

Adobe Analytics uses cookies to differentiate requests from different browsers and to store helpful information that an application can use later. They can also be used to associate browsing information with customer records.

Analytics uses cookies to define new visitors anonymously, help analyze clickstream data, and track historical activity on the website, such as response to particular campaigns or the length of the sales cycle.

| Cookie name | Expiration | Size | Location | Description |
| --- | --- | --- | --- | --- |
| **`s_ecid`** | 13 months | 45 bytes | First-party | Stores the Experience Cloud ID (ECID) or MID. Set by HTTP response. The MID is stored in `s_ecid=MCMID` format. Set after the client sets the AMCV cookie. It allows persistent first-party ID tracking and is used as a reference ID if the AMCV cookie expires. `SameSite` is set to "Lax". If you use the Web SDK to implement Adobe Analytics, the cookie expiration is set to 2 years; however, most modern browsers truncate the expiration to 13 months. |
| **`s_cc`** | Session | 4 bytes | First-party | Determines if cookies are enabled. Set by JavaScript. |
| **`s_sq`** | Session | 100-200 bytes | First-party | Used by Activity Map. It contains information about the previous link clicked by the visitor. Set by JavaScript. |
| **`s_vi`** | 2 years | 44 bytes | First-party, or `*.omtrdc.net` (third-party) | Stores a unique visitor ID and timestamp. Set by HTTP response. Each visitor ID is associated with a visitor profile on Adobe servers. Visitor profiles are deleted after 1 year of inactivity, regardless of any visitor ID cookie expiration. The `Secure` flag is set when `SameSite` is "None" and connection is HTTPS. `SameSite` is "Lax" by default for first-party cookies. `SameSite` is "None" when using third-party cookies, such as on `omtrdc.net` or `2o7.net`. Set `SameSite` to "None" when using a single CNAME to track multiple domains or properties. |
| **`s_fid`** | 2 years | 33 bytes | First-party | Stores the fallback unique visitor ID and timestamp. Set by JavaScript if the standard `s_vi` cookie cannot be set due to third-party cookie restrictions. Not used for first-party cookie implementations. |
| **`s_ac`** | Immediate | 1 byte | First-party | Helps determine the correct domain to set AppMeasurement cookies. Contains the static value `"1"`. Once this cookie is set, it is deleted immediately. |

## Cookies Set By Plug-ins

Some implementations make use of plug-ins, which are snippets of code that provide additional functionality for Analytics. These plug-ins can set cookies that are not listed above. See [Analytics plug-ins overview](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/plugins/impl-plugins) for a list of available plug-ins and what cookies that they set.

## Consequences of deleting Analytics cookies

If a visitor deletes their Analytics cookies, consider the following:

* **Visitor identification is lost:** When cookies are deleted, Adobe Analytics cannot recognize returning visitors. The next time the user visits your site, they are counted as a new visitor. [Cross-device Analytics](https://experienceleague.adobe.com/en/docs/analytics/components/cda/overview) can help mitigate this impact.
* **Session continuity is broken:** Any session-based or multi-visit analysis (such as attribution or conversion tracking) is disrupted. Events and conversions that happen after cookie deletion cannot be tied to previous activities by the same user.
* **Personalization and segmentation are affected:** Segments or personalized experiences based on visitor history or behavior are reset, as previous data is no longer associated with their current visit.
* **Cross-domain tracking is interrupted:** For third-party cookies, deleting them prevents Adobe Analytics from linking user activity across multiple domains that you own.
