---
title: Account Preferences and Notifications
description: Learn about user profiles, account preferences, and product usage data in Experience Cloud. Subscribe to product notifications for email and [!DNL Slack], and set up product alerts.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
TQID: https://experienceleague.adobe.com/2IL6hUlA1oNxJIFMwbVQUbxEGkJoghVUTyMi5wSRBsE
product_v2:
  - id: d0a3eab4-7b10-4d96-a71e-6c0f8e7b7c87
    internal-label: Experience Cloud
feature_v2:
  - id: e1eba07e-ab89-466f-9ab5-ceb891d7a67d
    internal-label: Account preferences and notifications
  - id: fdbb8fc9-ffa3-4b86-88fe-aa4c5a3e1bc6
    internal-label: Administration
subfeature_v2:
  - id: b75843fa-0a67-4a44-a6b1-cc627b0481dc
    internal-label: Support
  - id: bdea9bc8-5600-45db-b85e-d74bb59dfcff
    internal-label: Organizations (AEC)
  - id: dc42f745-24d2-44a4-99c3-dece518fa4bc
    internal-label: Alerts
  - id: eaef3029-0844-43fe-9e1c-7666a24f4d03
    internal-label: Subscriptions
  - id: eb1ae5c4-ef16-4998-851c-73cc9f0b7f06
    internal-label: Notifications
  - id: fef08361-6ac5-460c-93fe-d063e40b6a49
    internal-label: Getting started
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Account preferences and notifications 

To find Experience Cloud preferences, click **[!UICONTROL Profile]** ![preferences](../assets/preferences-icon-sm.png) in the header, then click **[!UICONTROL Preferences]**.

![preferences](../assets/preferences-navigation.png){width="100" zoomable="yes"}

On the [!UICONTROL Experience Cloud preferences] page, you can manage the following account features:

| Feature | Description |
|--- |--- |
|[!UICONTROL Profile]|Update your [Adobe Account Profile](https://account.adobe.com/profile). <p>Your profile photo and name appear when you log in to Adobe.com, Adobe products and services, and on public-facing sites like [!DNL Behance].|
|[!UICONTROL General]|Select an [organization](../administration/organizations.md).<p>This organization is the default one used when you sign-in to Experience Cloud. |
|[!UICONTROL Product usage data]| You can control what product usage data is shared with Adobe when using Experience Cloud applications. This is data about how you use our products, not your organization's content or data itself. Adobe uses this information to help improve our products, provide you with enhanced in-product support, and to personalize your experience and communications from us. <p>To learn more, see [Product usage data](#product-usage-data) (on this page).|
|[!UICONTROL Notifications]| Configure how and when you would like product [notifications](#subscribe-to-notifications-in-experience-cloud) and alerts: <ul><li>Select the products to which you want to subscribe for alerts</li><li>Configure the type of notification ([!UICONTROL in-app], [!UICONTROL email], or [Slack](#slack-notifications))</li><li>Specify the frequency at which you would like to receive notification emails. (Not sent, instant, daily, or weekly.)</li><li>Determine the alert priority. In-app alerts appear in the top-right corner of your window for a few seconds. Or, you can specify whether alerts should display until you dismiss them.</li></ul>|

## [!UICONTROL Product usage data] 

Product usage data that you choose to share with Adobe includes the following types of information about how you use and interact with Adobe applications:

* Browser and device information, such as device model and operating system, software and hardware information, browser and device settings, unique identifiers (such as IP address, cookie ID, or device ID), amount of memory installed, language settings, and screen resolution;
* How you interact with Adobe Experience Cloud apps, including the features you use and the options you select;
* Adobe product information, such as version number;
* Information about your content and documents such as number of pages and unique identifiers, but not the content itself;
* Content usage information such as how many times you access content and how you interact with your content within the app;
* Crash and error logs.

Adobe uses this information to help improve our products, provide you with support both in-product and via customer care, and to personalize your experience and communications from us. Learn more about [personalized experiences](personalized-learning.md).

## Subscribe to notifications in Experience Cloud 

You can select the products and categories to which you would like to subscribe. Notifications appear in the [!UICONTROL Notifications] popover (in-app), or in your email, or in [Slack](#slack-notifications) (depending on your subscriptions).

Email and Slack notifications are useful for situations when you are not signed in to Experience Cloud. 

### Subscribe to in-app and email notifications

1. Navigate to Experience Cloud [preferences](https://experience.adobe.com/preferences).

1. Under **[!UICONTROL Notifications]**, enable **[!UICONTROL In-app]** or **[!UICONTROL Email]**.

   Changes to notifications are saved automatically.

### Subscribe to [!DNL Slack] notifications 

You can configure your account preferences to send Experience Cloud notifications to a [!DNL Slack] channel. 

**Prerequisites**

* You must have an Experience Cloud account.
* You must have a [!DNL Slack] account. Your [!DNL Slack] administrator enables the Experience Cloud integration with [!DNL Slack].
* You must be a part of at least one [!DNL Slack] workspace.

**To subscribe to [!DNL Slack] notifications**

1. Navigate to Experience Cloud [Preferences](https://experience.adobe.com/preferences).

1. Locate [!DNL Slack], then click **[!UICONTROL Add to Slack]**.

   ![Add to Slack](../assets/add-to-slack.png)

   If [!DNL Slack] is installed, the application opens and a permission request message displays. If Slack is not installed, you must [request permission](#slack-troubleshoot).

1. Click **[!UICONTROL Allow]**.

1. Under **[!UICONTROL Notifications]**, enable [!DNL Slack] notifications for your desired products and categories.

   ![Slack notifications](../assets/slack.png)

   Updates to notifications are automatically saved.

### Request permission in [!DNL Slack] (troubleshooting) 

If [!DNL Slack] is not installed, a _[!UICONTROL Request to install]_ message displays when Slack opens after you click **[!UICONTROL Add to Slack]**. For example:

   ![Request Slack Integration](../assets/slack-workspace.png)

**To request permissions in Slack**

1. In [!DNL Slack], select the workspace from the **[!UICONTROL Workspace]** menu (top right corner).
   
1. To request application approval for the [!DNL Slack] workspace manager, click **[!UICONTROL Submit]**.
   
1. You will receive a notification in [!DNL Slack] after the application request is approved.
   
1. After you receive [!DNL Slack] approval, return to Experience Cloud **[!UICONTROL Notifications]** and follow the steps to [subscribe to Slack](#slack-notifications) (described above).

### What you will see in [!DNL Slack]

After successfully integrating [!DNL Slack], the [!DNL Slack] notifications display the following information:

* The personal message will be received from the application name _Adobe [!DNL Experience Cloud]_.
* The message includes the product logo for the particular application, such as Adobe [!DNL Experience Platform], Adobe [!DNL Experience Manager], and so on.
* A link to view all notifications on Experience Cloud.
* A link to manage notification preferences on Experience Cloud. 

## View [!UICONTROL notifications] and announcements in Experience Cloud 

In the [!DNL Experience Cloud] header, you can view notifications to which you [subscribed](#notifications), as well as view announcements.

1. Click the bell icon in the header. ![Notifications and Announcements](../assets/bell-icon.png)

1. Click **[!UICONTROL Notifications]** or **[!UICONTROL Announcements]**.

   This location is where you receive important information about products, your collaboration with fellow users, and other relevant updates. Updates include product releases, maintenance notices, shared items, and approval requests.

