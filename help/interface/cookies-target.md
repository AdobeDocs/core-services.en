---
description: Learn how Adobe Target uses cookies to give website operators the ability to test which online content and offers are more relevant to visitors.
solution: Experience Cloud,Analytics,Target
title: Adobe Target cookies 
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
---
# Adobe Target cookies

[!DNL Adobe Target] uses cookies to give website operators the ability to test which online content and offers are more relevant to visitors.

>[!NOTE]
>
>The information in this article applies to the [[!DNL Target] at.js JavaScript library](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} only.
>
>For information about cookies used in a [!DNL Target] implementation using the [[!DNL Adobe Experience Platform Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html){target=_blank}, see "Does the [!DNL Adobe Experience Platform Web SDK] use cookies? If so, what cookies does it use?" in [Frequently Asked questions in the DNL Platform Web SDK overview guide](https://experienceleague.adobe.com/docs/experience-platform/edge/web-sdk-faq.html){target=_blank}.
>
>You can change settings discussed in this article if needed, except for the cookie duration. [Consult your account representative](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} when changing cookie settings.
>
>[!DNL Target] users can also create customized third-party cookies.

## First-party cookies

The following first-party cookies are stored on the customer's domain:

|Cookie|Details|
| --- | --- |
|mbox|Stores anonymous identifiers about the visitor.<P>**Cookie domain**: The domain from which you serve the mbox. Because this cookie is served from your company's domain, the cookie is a first-party cookie. Example: `mycompany.com`. If any of your domain names include a country code, such as `mycompany.co.uk`, work with your Client Services to configure at.js to support this code. For information about customizing the cookie domain, if necessary, see "`cookieDomain`" under [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} in the *[!DNL Adobe Target] Developer Guide*.<P>**Server domain**: `clientcode.tt.omtrdc.net`, using the client code for your [!DNL Target] account.<P>**Cookie duration**: The cookie remains on the visitor's browser two years from the last login. You cannot change the cookie duration.<P>The cookie keeps some values to manage how your visitors experience [!DNL Target] activities:<P>**session ID**: A unique identifier for a given user session. By default the session expires after 30 minutes of inactivity. If you are generating `sessionId` yourself (for example, for [server-side implementations](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), ensure the following:<ul><li>The session ID can be any printable string except a space, question mark ( ? ), or a forward slash ( / ).</li><li>The session ID should be from 1 to 128 characters in length.</li><li>For a particular session, the cookie's value must stay the same across multiple requests.</li><li>You should never have parallel sessions (distinct `sessionIds`) for a given visitor at any point in time.</li></ul>Routing to a particular node in the edge cluster is done using session ID.<ul><li>The session is active for 30 minutes on the server side. Therefore, you shouldn't use a different session Id for a particular `tntId/thirdPartyId` within 30 minutes of the last request made with the `tntId/thirdPartyId`. Otherwise, changes to the profile could be inconsistent and unpredictable.</li><li>A new session ID must be used after thirty minutes of inactivity from a visitor.</li><li>Using the same session ID with multiple `tntIds/thirdPartyIds` can cause unpredictable changes to the profiles identified by the `tntId/thirdPartyIDs`.</li></ul>NOTE: See [limit on number of concurrent requests](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html?lang=en#content-delivery){target=_blank} for a given session ID.<P>**pc ID**: A semi-permanent ID for a visitor's browser. Lasts until cookies are manually deleted.<P>**check**: A simple test value used to determine if a visitor supports cookies. Set each time a visitor requests a page.<P>**disable**: Set if a visitor's load time exceeds the timeout configured in the at.js file. By default, this timeout lasts one hour.|
|at_check|Temporary cookie to check if the cookie read/write capability is enabled on the browser.|
|mboxEdgeCluster|This cookies is only present when/if [overrideMboxEdgeServer setting](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} is set to `true`.|

It is not possible to use HTTPOnly on the these first-party cookies. The at.js JavaScript library needs to read/write to these cookies. These cookies are created by at.js and are not set from the server.

The `secure` setting can be enabled on all of these cookies using the `secureOnly: true` configuration in the at.js implementation.

## Third-party cookies

The following third-party cookies are stored on `tt.omtrdc.net`:

|Cookie|Details|
| --- | --- |
|customerclientcode!mboxPC|This cookie is present if cross domain is enabled.|
|customerclientcode!mboxSession|This cookie is present if cross domain is enabled.|

These third-party cookies are HTTPOnly out of the box and are set by the [!DNL Target] edge servers.

The `secure` setting can be enabled on all of the cookies using the `secureOnly: true` configuration in the at.js implementation. 