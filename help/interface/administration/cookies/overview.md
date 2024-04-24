---
description: Learn how solutions and services in Adobe Experience Cloud use cookies.
title: How Cookies Are Used in Experience Cloud 
uuid: 4255a13a-917b-4b5f-a7d4-4b2e7521d189
---

# Cookies Used in Experience Cloud

Many services within the Adobe Experience Cloud use cookies. A cookie is a small piece of data that is presented by a website to a web browser. The browser stores this piece of data, and then returns it to the website that provided it. This action is performed with each subsequent request for pages and images.

Cookies are provided to maintain information during and sometimes between visits to a website. Cookies enable devices to be uniquely differentiated from other browsers who view the site.

>[!NOTE]
>
>Laws, regulations, and self-regulatory principles require you to obtain consent from visitors before you can store or retrieve information on a computer or other web connected device. Adobe suggests that you review with your counsel what laws, regulations, and principles control your use of cookies.

This documentation describes the cookies used by the Suite and has been prepared to assist you with understanding your consent obligations.

# SSL/TLS Certificate Licensing

Adobe recommends that you manage your certificate at no additional cost through the [Adobe Managed Certificate Program](https://experienceleague.adobe.com/docs/core-services/interface/ec-cookies/cookies-first-party.html). The Adobe Managed Certificate prorgram is fully automated and ensures certificates are renewed in a timely manner so that there is no impact due to expired certificates.

If you use choose not to use the [Adobe Managed Certificate Program](https://experienceleague.adobe.com/docs/core-services/interface/ec-cookies/cookies-first-party.html) you are responsible for providing a SSL/TLS certificate to be used for first-party cookies.  

If you provide your own certificate, it is your responsibility to purchase and maintain it.  Your SSL/TLS certificate must include an unlimited server license. 

In order to ensure certificate security, obtain a certificate signing request [CSR] from Adobe and arrange with your desired Certificate Authority to have the certificate signed.  Provide Adobe with the signed certificate for implementation.  By following this process, the security of the certificate's key is maintained.  Adobe Customer Care will assist in this process.

As part of certificate maintenance, at least one month prior to the expiration of your certificate, arrange with your desired certificate authority to obtain a renewed certificate and provide this to Adobe.  This certificate should use the same CSR used previously.  Contact Adobe if you need a copy of the CSR or would like a new CSR generated with a new key.

Customer Care can be reached at customercare@adobe.com or 1-800-497-0335.

Commonly used certificate authorities include DigiCert, Comodo and GeoTrust.

## About first-party cookies

Adobe Experience Cloud services use cookies to provide information on variables and components that do not persist between image requests and browser sessions. Where possible, Adobe uses first-party cookies to record activities on your site. To record activity on different sites such as other domains you may own, third-party cookies are required.

Many browsers and anti-spyware applications are designed to reject and delete third-party cookies. Adobe ensures that cookies can always be set even if third-party cookies are blocked. The specific behavior varies depending on whether you are using the Experience Platform Identity Service (ECID Service) or Analytics' legacy identifiers (such as the `s_vi` cookie):

* The [Experience Platform Identity Service (ECID Service)](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) automatically sets first-party cookies regardless of whether your collection domain matches your site domain. If they do not match, the Identity Service uses JavaScript to set cookies on your site's domain.
* If you use [Analytics legacy identifiers](analytics.md) (such as the `s_vi` cookie), it depends on how you have configured your data collection server. If the data collection server matches your site's domain, then cookies are set as first-party. If the collection server does not match your current domain, then cookies are set as third-party. In this case, if third-party cookies are blocked, Analytics sets a first-party fallback id (`s_fid`) instead of the standard `s_vi` cookie.

If you would like to ensure your collection server matches your site's domain, you can use a CNAME implementation which will enable forwarding from a custom domain specified in your CNAME implementation to Adobe's collection servers. This involves changes to your company's DNS settings to configure a CNAME alias to pointing to an Adobe hosted domain. Please note that while various Adobe products support using a CNAME, in all cases the CNAME is used to a create a trusted first-party endpoint for a specific customer and is owned by that customer. If you control multiple domains, they may use a single CNAME endpoint to track users across their domains, but wherever the site domain does not match the CNAME domain cookies are set as third party.

>[!NOTE]
>
>Regardless of whether your collection domain matches your site domain, Apple's Intelligent Tracking Prevention (ITP) program makes the first-party cookies set by Adobe short-lived on browsers that are governed by ITP, which include Safari on macOS and all browsers on iOS and iPadOS. As of November 2020, cookies set via CNAME also have the same expiry as cookies set via JavaScript. This expiry is subject to change.

If you want to establish a CNAME for data collection and if your site has secure pages using the HTTPS protocol, you can work with Adobe to obtain an SSL certificate.

The SSL certificate issuance process can often be confusing and time consuming. As a result, Adobe established a partnership with DigiCert, an industry-leading Certificate Authority (CA), and developed an integrated process by which the purchase and management of these certificates is automated.

With your permission, we work with a CA to issue, deploy, and manage a new SHA-2 SSL certificate for you. Adobe continues to manage this certificate and ensure that an unexpected expiration, revocation, or security concern, does not threaten the availability of your organization's secure collection.

## Cookies and privacy

Maintaining customer privacy and data security are top priorities at Adobe. Adobe participates in multiple privacy organizations and cooperates with privacy regulators and self-regulatory principles. This cooperation includes the Digital Advertising Alliance AdChoices program to provide customers with information about how their information is used, and choices about its use.

Most of the cookies set by Experience Cloud products contain no personally identifiable information. These cookies and associated data are secure and used only for your company's reports, and to provide relevant content and advertisements. The data is not available to third parties or other Adobe customers, unless used in aggregated industry reports. For example, the [!DNL Digital Marketing Insight Report] analyzes aggregated and anonymous data across retailers.

Adobe does not merge browser-level information across companies. To protect the privacy and security of customers' data, some of the services within Experience Cloud offer companies the ability to use a separate set of cookies for each site tracked. Some of the Suite offerings also offer customers the ability to use their own domain name as the owner of the cookie. This practice creates an extra layer of privacy and security, as it makes the Experience Cloud cookies *first party cookies*, belonging permanently to the company's site.

Cookies can store and provide only the information that was previously deposited in them. They are not able to execute code or access other information stored on the computer. Also, web browsers restrict access to cookie data. Browsers enforce a cookie security policy that makes all cookie data available only to the website that originally set the information.

For example, data contained in cookies set from the Adobe.com website cannot be viewed by any other website other than Adobe.com.

The following diagram illustrates cookie usage for a standard image request: 

![Cookie usage for a standard image request](assets/CookiesProcessGraphic-01.png)

The following diagram illustrates cookie usage for a straight image request (used in scenarios where a JS file is not loaded): 

![Cookie usage for a straight image request](assets/CookiesProcessGraphic2.png)
