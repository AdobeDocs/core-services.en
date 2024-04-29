---
description: Learn about Adobe Advertising cookies for mapping ad engagement events to conversion events and, potentially, use that information to optimize ad bids.
title: Adobe Advertising cookies 
uuid: 2eec48a3-3e81-488e-8e30-5fd62885de0b
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: 6818edea-31b1-49fc-bca2-32828c7ca78d
---
# Adobe Advertising cookies

Adobe Advertising (formerly Adobe Advertising Cloud) uses cookies to map ad engagement events to conversion events and, potentially, to use that information to optimize ad bids.

>[!NOTE]
>
>The beta Adobe Advertising Javascript tag that uses the [Adobe Experience Cloud ID (ECID) Service](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) creates first-party [Experience Cloud](experience-cloud.md) `s_ecid` cookies, not Adobe Advertising cookies.

| Cookie name | Expiration | Size | Location | Description |
| --- | --- | --- | --- | --- |
| **`_lcc`** | 15 minutes | 52 bytes | `everesttech.net` | Stores IDs and timestamps of display clicks. Determines if a click event on a display ad applies to an Adobe Analytics hit. |
| **`_tmae`** | 1 year | 1 KB | `everesttech.net` | Stores encoded IDs and timestamps for ad engagements using DSP tracking. Includes user engagement with ads, such as ad last seen |
| **`adcloud`** | 1 year | 50-150 bytes | First-party | The timestamps of the visitor's last visit to your website and the visitor's last search click. Also stores the `ef_id` that was created when the visitor clicked an ad. Ties the visitor ID with relevant audience segments and conversions. Helps optimize page load times by avoiding unnecessary requests to Adobe. |
| **`ev_sync_*`** |  | 8 bytes | `everesttech.net` | The date when synchronization is performed in `yyymmdd` format. Syncs the Adobe Advertising visitor ID with the partner ad exchange. It is created for new visitors and sends a synchronization request when expired. Includes the cookies `ev_sync_ax`, `ev_sync_bk`, `ev_sync_dd`, `ev_sync_fs`, `ev_sync_ix`, `ev_sync_nx`, `ev_sync_ox`, `ev_sync_pm`, `ev_sync_rc`, `ev_sync_tm`, and `ev_sync_yh`. |
| **`everest_g_v2`** | 1 year | ~27 bytes | `everesttech.net` | Stores the browser and visitor ID. Created after a user initially clicks an ad. Used to map the current and subsequent clicsk with other events on your website. |
| **`everest_session_v2`** | Session | ~16 bytes | `everesttech.net` | Stores the current session ID. |
| **`ev_tm`** | 2 years | ~20 bytes | `everesttech.net` | Stores the Adobe Advertising Demand Side Platform (DSP) ID. Corresponds to the visitor ID in the `everest_g_v2` cookie. |
| **`id_adcloud`** | 91 days | 16 bytes | First-party | Stores the visitor ID. |

{style="table-layout:auto"}
