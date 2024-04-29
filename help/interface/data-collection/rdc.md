---
title: Regional data collection
description: Information on regional data collection
exl-id: 295e9736-2a58-48a8-9968-5dfa33b70d95
---
# Regional Data Collection

The Adobe Experience Cloud uses regional data collection (RDC) so that interactions between your visitors and Adobe happen as close to your visitors as possible. Data collected locally at an edge site is securely forwarded to a core site for processing. Once processed, the data is available to Adobe Experience Cloud products and services.

The regional data collection workflow provides several benefits:

* **Performance**: With RDC, your visitors connect to the closest edge site. This optimization provides the fastest response time, resulting in more accurate tracking and faster loading times.
* **Redundancy**: If there is a disruption in communication between any edge site and core site, Adobe's infrastructure saves data locally, then forwards it to the core site when communications are restored. Adobe can also route traffic to other edge sites if a specific location experiences interruptions.

RDC currently includes the following locations (subject to change):

## First-party data collection

| RDC Type | Data Collection Centers |
| --- | --- |
| Global (default) | Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney |
| Global + China* | China*, Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney |
| Americas only | Oregon, Virginia |
| Europe only | Ireland, Paris |
| Asia Pacific only | Mumbai, Singapore, Tokyo, Sydney |
| China only* | Beijing |

{style="table-layout:auto"}

_*China RDC requires the China Performance Optimization add-on package, and only applies to Adobe Analytics using AppMeasurement data collection. Other Experience Cloud services and Web SDK data collection are not supported. Contact your Adobe Account Team to learn more about the China Performance Optimization add-on package._

## Third-party data collection

Third-party data collection includes cookie domains that don't match your website domain. Examples include `adobedc.net`, `omtrdc.net`, and `2o7.net`.

| RDC Type | Data Collection Centers |
| --- | --- |
| Default | Oregon, Virginia, Ireland, Paris, Mumbai, Singapore, Tokyo, Sydney, China* |

{style="table-layout:auto"}
