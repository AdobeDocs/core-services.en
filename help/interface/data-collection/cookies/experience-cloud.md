---
description: Learn how the ID service is stored and used across Experience Cloud applications.
solution: Experience Cloud,Analytics,Target
title: Experience Cloud Cookies 
uuid: a4788c1c-0402-4fc8-b894-cd24fa794f4f
feature: Cookies
topic: Administration
role: Admin
level: Experienced
exl-id: bd9bea58-9987-40d6-84e0-da185388bbbb
---
# Experience Cloud cookies

Adobe Experience Cloud uses cookies to store a visitor ID that is used across Experience Cloud applications. These cookies specifically apply to accessing Adobe Experience Cloud applications on [experience.adobe.com](https://experience.adobe.com).

**Cookie Name: s_ecid**

<table id="table_FF4C70D3D4CC425BA65162D5A9504F7D"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Attribute </p> </th> 
   <th colname="col2" class="entry"> <p>Description </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Information Stored </p> </td> 
   <td colname="col2"> <p> Contains a copy of the Experience Cloud ID (ECID) or MID. The MID is stored in a key-value pair that follows this syntax, s_ecid=MCMID|&lt;ECID&gt; </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Expiration </p> </td> 
   <td colname="col2"> <p>2 years, though most modern browsers truncate to 13 months</p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Usage </p> </td> 
   <td colname="col2"> <p>This cookie is set by the customer's domain after the AMCV cookie is set by the client. The purpose of this cookie is to allow persistent ID tracking in the 1st-party state and is used as a reference ID if the AMCV cookie has expired. Check AMCV cookie here for more details. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Location </p> </td> 
   <td colname="col2"> <p>CNAME customers only. Not applicable for 3rd-party scenarios. Cookie is stored on your domain, the same domain used by CNAME and your Analytics image request. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Size </p> </td> 
   <td colname="col2"> <p>45 bytes </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> SameSite=Lax </p> </td> 
   <td colname="col2"> <p>Cookies with this setting are only sent when the domain displayed in the URL of the browser matches the domain of the cookie. This setting is the new default for cookies in Chrome.</p> </td> 
  </tr> 
 </tbody> 
</table>

**Cookie Name: AMCV_###@AdobeOrg**

The [Experience Platform ID Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) uses JavaScript to store a unique visitor ID in an `AMCV_###@AdobeOrg` cookie on the domain of the current website, where `###` represents a random string of characters, such as `AMCV_1FD6776A524453CC0A490D44%40AdobeOrg.` 

See also, [Cookies and the ID Service](https://experienceleague.adobe.com/docs/id-service/using/intro/cookies.html).

<table id="table_1883C0836C1E4AF5A262FBF5000C1B11"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>Attribute </p> </th> 
   <th colname="col2" class="entry"> <p>Description </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Information Stored </p> </td> 
   <td colname="col2"> <p> Unique visitor IDs used by Experience Cloud Solutions. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Expiration </p> </td> 
   <td colname="col2"> <p> 13 months </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Usage </p> </td> 
   <td colname="col2"> <p> This cookie is used to identify a unique visitor </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Location </p> </td> 
   <td colname="col2"> <p> This cookie is stored at the domain of the website (not the domain of the image request). </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> Size </p> </td> 
   <td colname="col2"> <p> Varies, most customers can expect this cookie to be around 200 bytes in length. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>No value added. Chrome defaults to Lax. </p> </td> 
   <td colname="col2"> <p> Cookies with this setting are only sent when the domain displayed in the URL of the browser matches the domain of the cookie. This setting is the new default for cookies in Chrome. </p> </td> 
  </tr> 
 </tbody> 
</table>
