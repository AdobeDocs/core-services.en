---
title: IP addresses used by the Adobe Experience Cloud
description: If your organization's firewall blocks IP addresses that originate from Adobe, use this list to update your firewall settings.
exl-id: e24a70e4-9ed4-4b87-8bab-4ed0aebedd1f
---
# IP addresses used by the Adobe Experience Cloud

Some firewall configurations block IP addresses originating from Adobe's data collection servers or servers responsible for accessing data. You can use this list of ranges to alter your organization's firewall settings to allow access and to send data from within your organization. This page includes both inbound systems (such as data collection) and outbound systems (such as data feeds in Adobe Analytics) that Adobe uses.

>[!IMPORTANT]
>
>While Adobe does its best to keep this document current, it cannot guarantee that the list of IP ranges remains the same. Possible changes include growth and expansion of the business, an Internet registry requires changes to Adobe's IP address space, or an Internet service provider stops functioning.

In addition to the IP address blocks listed below, individual Adobe Experience Cloud products have their own IP addresses that they use:

* [Adobe Analytics](https://experienceleague.adobe.com/en/docs/analytics/technotes/ip-addresses)
* Customer Journey Analytics

## All Adobe IP address blocks

The following table covers all Adobe-owned IP addresses. This table includes all Adobe employee offices and data centers run by Adobe globally. It does not include services hosted on public clouds.

| IP block (CIDR Notation) |
| --- |
| `63.140.32.0/19` |
| `66.117.16.0/20` |
| `66.235.128.0/19` |
| `130.248.0.0/16` |
| `172.82.192.0/18` |
| `185.34.188.0/22` |
| `192.243.240.0/22` |

{style="table-layout:auto"}

## Adobe Experience Cloud data collection and FTP IP address blocks

If your organization prefers to allow specific IP address ranges, you can reference the following table. It includes:

* Data collection servers for all Experience Cloud products
* FTP servers for all Experience Cloud products

All IP ranges in this section are included in the above table.

| Location | IP range (CIDR notation) |
| --- | --- |
| Australia | `63.140.55.0/24` |
| Australia | `63.140.56.0/23` |
| California | `63.140.32.0/23` |
| California | `63.140.34.0/24` |
| France | `63.140.62.0/23` |
| India | `66.117.20.0/24` |
| India | `66.117.22.0/23` |
| Japan | `130.248.169.0/23` |
| Japan | `63.140.50.0/23` |
| Japan | `66.117.31.0/24` |
| London | `66.235.156.0/24` |
| London | `185.34.188.0/22` |
| London | `130.248.152.0/22` |
| London | `130.248.244.0/23` |
| Oregon | `66.235.132.0/22` |
| Oregon | `130.248.130.0/23` |
| Oregon | `130.248.150.0/24` |
| Oregon | `130.248.160.0/21` |
| Oregon | `192.243.242.0/24` |
| Singapore | `130.248.170.0/23` |
| Singapore | `130.248.240.0/24` |
| Singapore | `63.140.44.0/22` |
| Singapore | `63.140.48.0/23` |
| Singapore | `66.117.30.0/24` |
| Singapore | `172.82.240.8/29` |
| Singapore | `172.82.240.88/29` |
| Virginia | `63.140.38.0/23` |
| Virginia | `63.140.54.0/24` |

{style="table-layout:auto"}

The Adobe Experience Cloud also supports IPv6 in limited capacity. These IP blocks serve similar data collection purposes as their IPv4 counterparts above, but do not include FTP.

| Location | Host |
| --- | --- |
| Australia | `2406:da1c:406:1a00::/56` |
| Australia | `2406:da1c:ce5:b400::/56` |
| California | `2600:1f1c:366:d900::/56` |
| France | `2a05:d012:706:d000::/56` |
| India | `2406:da1a:f34:6a00::/56` |
| Ireland | `2a05:d018:309:600::/56` |
| Japan | `2406:da14:b07:ab00::/56` |
| Oregon | `2600:1f14:1eb:7d00::/56` |
| Oregon | `2600:1f14:9d3:2b00::/56` |
| Singapore | `2406:da18:6e8:1e00::/56` |
| Virginia | `2600:1f18:1a20:e800::/56` |
| Virginia | `2600:1f18:4fd:6000::/56` |
| Virginia | `2600:1f18:b00:e100::/56` |
| Virginia | `2600:1f18:d1f:bd00::/56` |

>[!TIP]
>
>FTP connections for Adobe Analytics export features (including Data Warehouse and data feeds) only originate from IPv4 addresses in the London, Oregon, and Singapore locations.
