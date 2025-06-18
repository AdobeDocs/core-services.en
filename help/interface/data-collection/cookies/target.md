---
description: Learn how Adobe Target uses cookies to give website operators the ability to test which online content and offers are more relevant to visitors.
solution: Target
title: Adobe Target Cookies 
uuid: 44f7e32e-8d99-4682-8b54-8364d001b403
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: c4399cc0-8333-47b8-b830-2ba7359f464a
---
# Adobe Target cookies

Adobe Target uses cookies to give website operators the ability to test which online content and offers are more relevant to visitors.

>[!NOTE]
>
>The information in this article only applies to the [Adobe Target JavaScript library](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} (`at.js`). See [Adobe Experience Platform Web SDK cookies](web-sdk.md) for information on Target implementations using the Web SDK.
>
>You can change settings discussed in this article if needed, except for the cookie duration. [Consult your account representative](https://experienceleague.adobe.com/docs/target/using/cmp-resources-and-contact-information.html){target=_blank} when changing cookie settings.

## First-party cookies

The following first-party cookies are stored on the customer's domain:

|Cookie|Details|
| --- | --- |
|`mbox`|Stores anonymous identifiers about the visitor.<P>**Cookie domain**: The domain from which you serve the mbox. Because this cookie is served from your company's domain, the cookie is a first-party cookie. If any of your domain names include a country code, such as `example.co.uk`, work with Client Services to configure `at.js` to support this code. For information about customizing the cookie domain, if necessary, see `cookieDomain` under [targetGlobalSettings](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} in the Adobe Target developer guide.<P>**Server domain**: `clientcode.tt.omtrdc.net`, using the client code for your Adobe Target account.<P>**Cookie duration**: The cookie remains on the visitor's browser two years from the last login. You cannot change the cookie duration.<P>The cookie keeps some values to manage how your visitors experience [!DNL Target] activities:<P>**session ID**: A unique identifier for a given user session. By default the session expires after 30 minutes of inactivity. If you are generating `sessionId` yourself (for example, for [server-side implementations](https://experienceleague.adobe.com/docs/target-dev/developer/server-side/server-side-overview.html){target=_blank}), ensure the following:<ul><li>The session ID can be any printable string except a space, question mark ( ? ), curly braces ( { } ), or a forward slash ( / ).</li><li>The session ID should be from 1 to 128 characters in length.</li><li>For a particular session, the cookie's value must stay the same across multiple requests.</li><li>You should never have parallel sessions (distinct `sessionIds`) for a given visitor at any point in time.</li></ul>Routing to a particular node in the edge cluster is done using session ID.<ul><li>The session is active for 30 minutes on the server side. Therefore, you shouldn't use a different session Id for a particular `tntId/thirdPartyId` within 30 minutes of the last request made with the `tntId/thirdPartyId`. Otherwise, changes to the profile could be inconsistent and unpredictable.</li><li>A new session ID must be used after thirty minutes of inactivity from a visitor.</li><li>Using the same session ID with multiple `tntIds/thirdPartyIds` can cause unpredictable changes to the profiles identified by the `tntId/thirdPartyIDs`.</li></ul>NOTE: See [limit on number of concurrent requests](https://experienceleague.adobe.com/docs/target/using/troubleshoot/target-limits.html#content-delivery){target=_blank} for a given session ID.<P>**pc ID**: A semi-permanent ID for a visitor's browser. Lasts until cookies are manually deleted.<P>**check**: A simple test value used to determine if a visitor supports cookies. Set each time a visitor requests a page.<P>**disable**: Set if a visitor's load time exceeds the timeout configured in the at.js file. By default, this timeout lasts one hour.|
|`at_check`|Temporary cookie to check if the cookie read/write capability is enabled on the browser.|
|`mboxEdgeCluster`|This cookies is only present when/if [overrideMboxEdgeServer setting](https://experienceleague.adobe.com/docs/target-dev/developer/client-side/at-js-implementation/functions-overview/targetglobalsettings.html){target=_blank} is set to `true`.|

It is not possible to use `HTTPOnly` on the these first-party cookies. The `at.js` JavaScript library needs to read/write to these cookies. These cookies are created by `at.js` and are not set from the server.

The `secure` setting can be enabled on all of these cookies using the `secureOnly: true` configuration in `at.js`.

## Third-party cookies

Adobe Target users can create customized third-party cookies. The following third-party cookies are stored on `tt.omtrdc.net`:

|Cookie|Details|
| --- | --- |
| `customerclientcode!mboxPC` | Present if cross domain is enabled. |
| `customerclientcode!mboxSession` | Present if cross domain is enabled. |

These third-party cookies are HTTPOnly out of the box and are set by Adobe Target data collection servers.

The `secure` setting can be enabled on all of the cookies using the `secureOnly: true` configuration in `at.js`.
