---
description: Learn how set up secure certificates for use with Adobe Experience Cloud first-party cookies.
solution: Experience Cloud,Analytics
title: Adobe-managed certificate program
index: y
snippet: y
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: e15abde5-8027-4aed-a0c1-8a6fc248db5e
---
# Adobe-managed certificate program

The Adobe-managed certificate program is the recommended process for setting up first-party certificates needed for a CNAME implementation. The program is fully automated once configured. It renews certificates in a timely manner so that there is no impact to data collection due to expired certificates. The program is free for your first 100 CNAMEs.

If you currently manage your own certificates, you are responsible for purchasing, maintaining, and providing a certificate to Adobe for first-party cookie use. You can contact Adobe Customer Care to discuss migrating to the Adobe-managed certificate program.

## Implementation

Follow these steps to implement a new certificate for first-party data collection:

1. Download and fill out the [First-party domain request form](cookies/assets/First_Party_Domain_Request_Form.xlsx)

1. Open a ticket with Adobe Customer Care requesting to set up first-party data collection on the Adobe-managed certificate program. 

1. Upon receiving the ticket, the Adobe representative provides you with a CNAME record. These records must be configured on your company's DNS server before Adobe can purchase the certificate on your behalf. For example, the hostname `data.example.com` points to `hiodsibxvip01.data.adobedc.net`.

1. When the CNAME record is in place on your organization's servers, Adobe works with DigiCert to purchase and install a certificate on Adobe data collection servers.

## Validate hostname forwarding {#validate}

Once Adobe has installed the certificate, you can use one of the following methods to validate that it is working.

+++**Browser validation**

You can use any browser to validate that a certificate is installed correctly. Type your CNAME with `_check` as the path into the address bar. For example:

`data.example.com/_check`

If everything works, the browser shows `SUCCESS`. If the certificate is not installed correctly, you are issued a security warning.

+++

+++**Command line (`curl`)**

Most modern operating systems already have [`curl`](https://curl.se) installed.

Type the following into the command line:

```sh
curl data.example.com/_check
```

If everything works correctly, the console returns `SUCCESS`.

>[!TIP]
>
>You can use the `-k` flag to disable the security warning to help with troubleshooting.

+++

+++**Command line (`nslookup`)**

Type the following into the command line:

```sh
nslookup data.example.com
```

If everything works correctly, Adobe's data collection servers are returned:

```text
Server: hiodsibxvip01.corp.adobe.com
Address: 10.50.112.247

Name: example.com.ssl.d1.sc.omtrdc.net
Addresses: 63.140.37.126
    63.140.37.206
    63.140.36.51
    63.140.36.145
Aliases: smetrics.example.com
```

+++

## Update implementation code {#update}

Once you have validated that your certificate works correctly, you can update your Adobe implementation to use these values.

* For Adobe Analytics AppMeasurement implementations, update the [`trackingServer`](https://experienceleague.adobe.com/en/docs/analytics/implementation/vars/config-vars/trackingserver) configuration variable. If you have an existing implementation, see [Visitor migration](https://experienceleague.adobe.com/en/docs/analytics/technotes/visitor-migration) for additional steps on how to prevent existing visitors from being counted as new visitors.
* For Web SDK implementations, update the [`edgeDomain`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/edgedomain) property within the [`configure`](https://experienceleague.adobe.com/en/docs/experience-platform/web-sdk/commands/configure/overview) command.

## Maintenance and renewals

Thirty days before your first-party certificate expires, Adobe validates whether the CNAME is still valid and in use. If so, Adobe assumes that you want to continue using the service and automatically renews the certificate on your behalf. 

>[!IMPORTANT]
>
>If the CNAME has been removed or is no longer valid (Does not map to the provided Adobe secure hostname), Adobe cannot renew the certificate and the entry in Adobe's system is marked for removal without further communication.

## Frequently asked questions

+++Is this process secure?

Yes. The Adobe-managed certificate program is more secure than your organization providing Adobe with a certificate. No certificate or private key changes hands outside of Adobe and the issuing certificate authority.

+++

+++How can Adobe purchase a certificate for our domain?

The certificate can only be purchased when you have pointed the specified hostname to an Adobe-owned hostname. You essentially delegate this hostname to Adobe and allow Adobe to purchase the certificate on your behalf.

+++

+++Can I request that the certificate be revoked?

Yes. As the owner of the domain, you are entitled to request that the certificate is revoked. Contact Adobe Customer Care to start this process.

+++

+++What encryption type is used?

Adobe works with DigiCert to issue a SHA-2 certificate.

+++

+++Does this program incur any additional cost?

No. Adobe offers this service to all Adobe Experience Cloud customers at no additional cost.

+++

+++What cipher security levels does Adobe offer?

Adobe offers two cipher security levels to meet varying customer needs for security on first-party data collection. These levels determine which encryption algorithms are supported for HTTPS connections with Adobe servers. Adobe regularly reviews and updates the set of supported algorithms based on current security practices. If you would like to change your cipher security settings, contact Customer Care.
 
* **Standard** requires TLS 1.2 or newer and at least 128-bit encryption. It is designed to provide the widest device compatibility while maintaining secure encryption.
* **High** cipher security level requires TLS 1.2 or newer and removes support for weaker ciphers. It is designed for customers who desire the strongest encryption and are not concerned about support for older devices.

The following clients are known to be unable to connect with cipher security set to **High**:

* Windows 8.1 and earlier (last updated in 2018)
* Windows Phone 8.1 and earlier (last updated in 2016)
* OS X 10.10 and earlier (last updated in 2017)
* iOS 8.4 and earlier (last updated in 2015)

+++

+++What HTTPS certificate types are supported?

Adobe supports both RSA and ECC certificate types to meet varying customer needs. RSA certificates are more widely supported for clients, but ECC certificates use less processing on both the server and client side. For Adobe-managed certificates, both RSA and ECC are provided. For customer-managed certificates, both RSA and ECC are recommended. Modern clients support both RSA and ECC. The following clients are known to only support RSA certificates:

* Windows Vista and earlier (last updated in 2012)
* Windows Phone 8.0 and earlier (last updated in 2014)
* OS X 10.8 and earlier (last updated in 2013)
* iOS 5.1 and earlier (last updated in 2012)
* Android 4.3 and earlier (last updated in 2013)

+++
