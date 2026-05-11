---
description: Learn how to implement DNS prefetch to help reduce page load times with different applications and services in CX Enterprise.
solution: Experience Cloud
title: Use DNS Prefetch
uuid: 4220e223-e00e-46b1-8bde-52248913bea1
topic: Administration
role: Admin
level: Experienced
exl-id: caf2ff76-2076-436d-a5a7-aff531464480
TQID: 'https://experienceleague.adobe.com/uTXtbHEccwB-Nog-AJ282p59hHCppAsAyg5pgNRreR4'
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: CX Enterprise
feature_v2:
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id:
      id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
      internal-label: Support
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
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Use DNS prefetch

Implement DNS prefetch to help reduce page load times with different applications and services.

## Understanding DNS prefetch

Browsers use DNS prefetch to automatically resolve domain names linked on a Web page to their corresponding IP addresses. The prefetch process starts when your browser loads a web page. As an example, assume that your page contains a selectable link to `www.adobe.com`. When a browser loads this page, it uses the _DNS system_ to look up the linked domain name and resolve it to a corresponding numeric IP address. DNS prefetch helps improve page performance because the domain name is already resolved to an IP address before a site visitor clicks that link or button. The DNS prefetch process is transparent to the users. 

## DNS prefetch and Adobe CX Enterprise applications

DNS prefetch works automatically with static, embedded links on a page. This also means automatic DNS prefetch doesn't work with different [!UICONTROL CX Enterprise] applications and services because: 

* Each CX Enterprise application or service generates DNS calls dynamically as the page loads.
* The browser can't resolve domain names to IP address before these calls are made.

However, you can manually implement DNS prefetch with your CX Enterprise applications. You do this by adding the HTML `<dns-prefetch>` tag to the `<head>` section of your page code as shown below. When implemented properly, DNS prefetch can help save a few milliseconds of page load time. 

## DNS prefetch code samples

The following examples show you how to make DNS prefetch calls to different [!DNL CX Enterprise] applications and services. Some prefetch calls require your [!DNL Adobe] Organization ID or tracking server information. In these examples, the code in *italics* represents a variable placeholder. You would replace that code with your own [!DNL Adobe] partner ID, customer code, or tracking server information, and so on. 

* **Analytics:** `<link rel="dns-prefetch" href="//data.example.com">`. 

  Add a separate tag for each DNS name if you use non-secure and secure tracking servers. 

* **Audience Manager:** `<link rel="dns-prefetch" href="//dpm.demdex.net">` 

* **CX Enterprise ID Service:** `<link rel="dns-prefetch" href="//fast.examplepartnerid.demdex.net">` 

* **Advertising Cloud:** 

  * `<link rel="dns-prefetch" href="//pixel.everesttech.net">`    
  * `<link rel="dns-prefetch" href="//cm.everesttech.net">`    
    
* **[!DNL Target]:** `<link rel="dns-prefetch" href="//example.tt.omtrdc.net">`

>[!MORELIKETHIS]
>
>* [DNS Prefetching](https://www.chromium.org/developers/design-documents/dns-prefetching) on Chromium

