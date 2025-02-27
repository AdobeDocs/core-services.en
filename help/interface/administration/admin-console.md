---
title: User and Product License Management 
description: Manage users and product licenses in Admin Console for Experience Cloud applications.
application: Experience Cloud
index: yes
feature: Admin Console
topic: Administration
role: Admin
level: Experienced
exl-id: c82821c4-aa5d-48ae-8bef-5937fede8db2
---
# User management and product licenses

This page provides information specifically for Experience Cloud administrators, with links to common user and product management documentation. 

For general identity management help applicable to all Adobe applications, see the [Enterprise and teams admin guide](https://helpx.adobe.com/enterprise/admin-guide.html).

## Administrative roles in Admin Console

The Admin Console provides three primary administrative roles, each with specific levels of access and responsibility:

| Help link |  Description |
| ------- | ------- |
|System administrator |Full access - Manages all aspects of the console. <br>Key responsibilities: <br><ul><li>Add, remove, and manage users.</li><li>Assign and revoke product licenses.</li><li>Configure identity and authentication settings</li><li>View and manage billing information.</li><li>Set up additional admins and delegate roles.</li></ul> **Best for:** IT administrators or team leads overseeing the entire organization's Adobe environment. |
|Product administrator |Product-specific management - Controls access and permissions for specific Adobe products.<br>Key responsibilities:<ul><li>Assign and manage licenses for a specific product.</li><li>Create and manage product profiles.</li><li>Add or remove users within assigned products.</li></ul>   **Best for:** Teams/users managing specific software like Marketo Engage or Adobe Creative Cloud.|
|Product profile administrator |Granular role management - Focuses on managing user groups and permissions within a product.<br>Key Responsibilities:<ul><li>Create and manage product profiles.</li><li>Assign permissions and feature access within profiles.</li><li>Add or remove users within profiles.</li></ul> **Best for:** Department leads or team managers overseeing smaller groups with specialized needs. <br> Administrators can combine roles for greater flexibility, depending on organizational requirements.|

## Admin Console for Experience Cloud 

To manage identity and product licenses for Experience Cloud applications, navigate to the [Admin Console](https://adminconsole.adobe.com/enterprise/).

Here are resources you might need when getting started as an administrator in Admin Console:

### Setup tasks

| Help link |  Description |
| ------- | ------- |
|[Set up identity and single sign-on](https://helpx.adobe.com/enterprise/using/set-up-identity.html) | **[!UICONTROL  Admin Console]** > **[!UICONTROL Settings]** <br>Learn how to set up your users' accounts with different ID types with or without single sign-on (SSO). Set up SSO for Adobe software, configure SAML settings, and go through the most common questions and errors. |
|[Set up organization via directory trust](https://helpx.adobe.com/enterprise/using/directory-trust.html)  | Authenticate your users against a domain already claimed by another organization. For information about finding and switching organizations, see [Organizations in Experience Cloud](organizations.md).  |
|[Authentication settings (enterprise)](https://helpx.adobe.com/enterprise/using/authentication-settings.html)  |Admin Console supports several password protection levels and policies to ensure safety and security. You can specify to use a password protection level to apply to all users across your organization.  |
| [Privacy and security contacts](https://helpx.adobe.com/enterprise/using/security-contacts.html)  | Protect your organization's and users' data. If a security incident involving our software solutions occurs, notifications are sent to the appropriate compliance officers. Enterprises have personnel whose role is specific to data protection, integrity, and other compliance matters. Therefore, contact information for such personnel is critical to help ensure prompt notification in the event of a security incident.|

### User management

| Help link | Description |
| ------- | ------- |
|[Manage multiple users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) |**[!UICONTROL Admin Console]** > **[!UICONTROL Users]** <br>Learn how to manage multiple users via CSV bulk upload to the Admin Console.  |
| [Identity Types](https://helpx.adobe.com/enterprise/using/identity.html) | Identity types allow the organization different levels of control over the users' accounts and data. Your choice of identity model impacts how your organization stores and shares assets. While Federated ID and Enterprise ID models are created and managed by the organization, Adobe IDs are created and managed by the individual.  |
|[User Sync Tool](https://helpx.adobe.com/enterprise/using/user-sync.html) (UST)  |The Adobe User Sync Tool is a desktop application used to automate syncing user data between an organization's identity management system (like Active Directory) and Adobe Admin Console. The tool allows administrators to streamline user provisioning, updates, and deactivation across Adobe products.  |
|[View user details (Admin Tool)](admin-tool-experience-cloud.md)  | View a sortable and filterable list of all Experience Cloud users and policies with details in the [!UICONTROL Admin Tool]. |

### Reports and logs

| Help link | Description |
| ------- |------- |
| [Audit log](https://helpx.adobe.com/enterprise/using/audit-logs.html) |**[!UICONTROL Insights]** > **[!UICONTROL Logs]** > **[!UICONTROL Audit Log]** <br> Track all changes made in the Admin Console. |


## Application-specific resources

These links help you find administration information for specific Experience Cloud applications.

<!-- | Application | Link to resource|
| ------- | ------- |
|  [!DNL Analytics] <p>Customer Journey Analytics| [Analytics in the Adobe Admin Console overview](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home) <p>[Administration requirements](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace) |
| [!DNL Audience Manager] | [Audience Manager user migration to Admin Console](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration) |
| [!DNL Campaign] v8 |  [Get started with permissions](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) |
| [!DNL Campaign Standard] to [!DNL Campaign v8] | [User access management from Campaign Standard to Campaign V8](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs) |
| [!DNL Commerce] | [Configure the Commerce Admin Integration with Adobe ID](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config) |
| [!DNL Dynamic Media Classic] | [Administration setup](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration) |
| [!DNL Experience Manager as a Cloud Service] |  [Accessing the Admin Console](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) |
| [!DNL Experience Platform] <p>[!DNL Data Collection] | [Access control UI overview](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) <p>[Permission management for data collection in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)|
| [!DNL GenStudio for Performance Marketing] | [Provision Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning) |
| [!DNL Journey Optimizer] | [Manage users and roles](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions) |
| [!DNL Journey Optimizer B2B Edition] | [User management](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management) |
|[!DNL  Journey Orchestration] | [Access management](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management) |
| [!DNL Marketo Engage] | [Understanding Marketo Subscription and User Migration to the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) |
| [!DNL Marketo Measure] | [Adobe Admin Console Setup](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup) |
| [!DNL Mix Modeler] | [Access controls](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls) |
| [!DNL Pass] | [Get started with Account IQ](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started) |
| [!DNL Target] | [Administrator first steps](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target) <p> [User management](https://experienceleague.adobe.com/en/docs/target/using/administer/manage-users/user-management) |
| [!DNL Workfront] | [Manage users in the Adobe Admin Console](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console) |

 -->

* [Analytics](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-console/home) 
* [Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/workspace-faq/frequently-asked-questions-analysis-workspace) 
* [Audience Manager](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/features/administration/admin-console-migration) 
* [Campaign v8](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) 
* [Campaign Standard](https://experienceleague.adobe.com/en/docs/campaign-web/acs-to-ac/user-management-acs) 
* [Commerce](https://experienceleague.adobe.com/en/docs/commerce-admin/start/admin/ims/adobe-ims-config) 
* [Dynamic Media Classic](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/setup/administration-setup#user_administration) 
* [Experience Manager as a Cloud Service](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/onboarding/journey/admin-console) 
* [Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/ui/overview) and [Data Collection](https://experienceleague.adobe.com/en/docs/experience-platform/collection/permissions)
* [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/product-provisioning) 
* [Journey Optimizer](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/access-control/permissions) 
* [Journey Optimizer B2B Edition](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/admin/user-management) 
* [Journey Orchestration](https://experienceleague.adobe.com/en/docs/journeys/using/starting-with-journeys/access-management) 
* [Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console) 
* [Marketo Measure](https://experienceleague.adobe.com/en/docs/marketo-measure/using/configuration-and-setup/getting-started-with-marketo-measure/adobe-admin-console-setup) 
* [Mix Modeler](https://experienceleague.adobe.com/en/docs/mix-modeler/using/data-governance/access-controls)
* [Adobe Pass](https://experienceleague.adobe.com/en/docs/pass/aiq-help/get-started)
* [Target](https://experienceleague.adobe.com/en/docs/target/using/administer/start-target)
* [Workfront](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/add-users/create-manage-users/admin-console)

The majority of Admin Consol help for all Adobe applications is documented in [Enterprise and teams admin guide](https://helpx.adobe.com/enterprise/admin-guide.html).
