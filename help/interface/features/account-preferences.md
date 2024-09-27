---
title: Account Preferences and Notifications
description: Learn about user profiles and account preferences in Experience Cloud. Subscribe to product notifications for email and [!DNL Slack], and set up product alerts.
solution: Experience Cloud
feature: Account Preferences, Notifications, Alerts
topic: Administration
role: Admin
level: Intermediate
exl-id: 1e34c6b2-a792-41c4-adb7-583de596237f
---
# Account preferences and notifications {#preferences}

To find Experience Cloud preferences, click your **[!UICONTROL User Account]** ![preferences](../assets/preferences-icon-sm.png) icon, then click **[!UICONTROL Preferences]**.

On the [!UICONTROL Experience Cloud preferences] page, you can manage the following account features:

| Feature | Description |
|--- |--- |
|Profile|Update your [Adobe Account Profile](https://account.adobe.com/profile). <p>Your profile photo and name appear when you log in to Adobe.com, Adobe products and services, and on public-facing sites like [!DNL Behance].|
|General|Select an [organization](../administration/organizations.md).<p>This organization is the default one used when you sign-in to Experience Cloud. |
|[!UICONTROL Product data collection]|Select which technologies Adobe can use to collect data on how you use your Adobe products. |
|Notifications| Configure how and when you would like product [notifications](#subscribe-to-notifications-in-experience-cloud) and alerts: <ul><li>Select the products to which you want to subscribe for alerts</li><li>Configure the type of notification ([!UICONTROL in-app], [!UICONTROL email], or [Slack](#slack-notifications))</li><li>Specify the frequency at which you would like to receive notification emails. (Not sent, instant, daily, or weekly.)</li><li>Determine the alert priority. In-app alerts appear in the top-right corner of your window for a few seconds. Or, you can specify whether alerts should display until you dismiss them.</li></ul>|
|[!UICONTROL Personalized learning recommendations and promotions]|Select where you would like to receive [personalized help](personalized-learning.md) for your Adobe products. This help is available via email, in-product, and the Experience League Communities. |

## Subscribe to notifications in Experience Cloud {#notifications}

You can select the products and categories to which you would like to subscribe. Notifications appear in the [!UICONTROL Notifications] popover (in-app), or in your email, or in [Slack](#slack-notifications) (depending on your subscriptions).

Email and Slack notifications are useful for situations when you are not signed in to Experience Cloud. 

### Subscribe to in-app and email notifications

1. Navigate to Experience Cloud [preferences](https://experience.adobe.com/preferences).

1. Under **[!UICONTROL Notifications]**, enable **[!UICONTROL In-app]** or **[!UICONTROL Email]**.

   Changes to notifications are saved automatically.

### Subscribe to [!DNL Slack] notifications {#slack}

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

### Request permission in [!DNL Slack] (troubleshooting) {#slack-troubleshoot}

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

## View [!UICONTROL notifications] and announcements in Experience Cloud {#view-notifications}

In the [!DNL Experience Cloud] header, you can view notifications to which you [subscribed](#notifications), as well as view announcements.

1. Click the bell icon in the header. ![Notifications and Announcements](../assets/bell-icon.png)

1. Click **[!UICONTROL Notifications]** or **[!UICONTROL Announcements]**.

   This location is where you receive important information about products, your collaboration with fellow users, and other relevant updates. Updates include product releases, maintenance notices, shared items, and approval requests.
