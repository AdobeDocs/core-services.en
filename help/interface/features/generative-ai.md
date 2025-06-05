---
title: Generative AI in Experience Cloud Applications
description: Learn about generative AI (GenAI) and how Experience Cloud applications use GenAI and [!DNL AI Assistant]. 
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
---
# Generative AI in Experience Cloud products

Generative AI (genAI) in Experience Cloud helps you automate creative and cognitive tasks and enhance productivity. This page describes where Experience Cloud applications support genAI and AI Assistant, and provides links to learn more about these features.

**What is genAI?**

Generative AI is a type of AI that can create original content. For example, it can create text, images, video, audio, or software code in response to a user's prompt or request.

* **Create:** The ability to generate content (text, images, music, or videos) from scratch, based on its training and input prompts. This ability is the _generative_ aspect of generative AI.

* **Generate a response:** AI provides an answer or reaction to a prompt, typically drawing on its available data and knowledge repositories.

**What is [!DNL AI Assistant]?**

[!DNL AI Assistant] is a conversational tool supported in Experience Platform and related applications. Use it to quicktly gain _product knowledge_ and _operational insights_ in supported products.

* **Product knowledge:** Product knowledge refers to concepts and topics grounded in Experience League documentation. Learn how to create effective, [objective-based prompts](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to get the most out of [!DNL AI Assistant]. All responses from Experience League are verifiable and cited with links.

* **Operational insights:** [Operational insights](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions#objects-questions) refer to generated responses about your metadata objects (attributes, audiences, dataflows, datasets, and so on). With [!DNL AI Assistant], you can accomplish in seconds what otherwise might take hours or days.

* **Customer support**: The [Product Support Agent](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/new-features/customer-support) is a self-serve debugging and troubleshooting capability of [!DNL AI Assistant] that you can use for Experience Platform features and applications. Troubleshoot support issues without leaving your workflows, create customer support tickets, and track case progress using AI Assistant. 

    **Note:** This feature is in Alpha and may not be available to your organization. To participate in the Alpha program and access this feature, contact your Adobe Account Team.

[Learn about AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) 

## GenAI availability in Experience Cloud products {#products}

The following Experience Cloud applications support generative AI or [!DNL AI Assistant]. Support for Adobe Firefly is also indicated per product.

Updated: **June 5, 2025**

* [[!DNL GenStudio for Performance Marketing]](#gspm)
* [[!DNL Experience Manager]](#aem)
* [[!DNL Journey Optimizer]](#journey-optimizer)
* [[!DNL Journey Optimizer] B2B Edition](#ajo-b2b)
* [[!DNL Campaign] Managed Cloud Services](#campaign-cs)
* [[!DNL Customer Journey Analytics]](#cja)
* [[!DNL Real-Time CDP]](#rtcdp)
* [[!DNL Marketo]](#marketo)
* [[!DNL Workfront]](#workfront)

## GenStudio for Performance Marketing {#gspm}

[!DNL GenStudio for Performance Marketing] is a generative AI application designed to help enterprise marketing teams create, activate, and optimize on-brand campaign content across channels like paid media, email, and display ads. 

Performance marketers can use natural language prompts to generate personalized, brand-compliant assets. GenStudio for Performance Marketing accelerates campaign execution, scales content production without compromising brand integrity, and provides performance analytics for improving overall ROI.

[Learn more](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)

Adobe Firefly compatibility: **Yes**

## [!DNL Experience Manager] {#aem}

The following sections briefly describe generative AI in AEM applications.

### Experience Manager Sites

In AEM Sites, you can use _[!UICONTROL Generate Variations]_. This feature uses generative artificial intelligence to create content variations based on your input prompts. Prompts are either provided by Adobe or created and managed by you.

After creating variations, you can use the content on your website and measure its success using the [Experimentation](https://www.aem.live/docs/experimentation) feature in Edge Delivery Services. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly.

**Input and output examples**

Input fields include: 
 
* Number of Variations to generate
* Audience Source
* Audience Target
* Additional Context
* Customer-driven prompts 

The output is generated content or market copy. 

Adobe Firefly compatibility: **Yes**

[Learn more](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor)

### Sites Optimizer {#sites-optimizer}

AEM Sites Optimizer uses generative AI to analyze and improve the performance and effectiveness of web experiences. These insights are grouped into key opportunity areas: Engagement, Traffic Acquisition, Security Posture, and, Site Health. Each category highlights specific ways to enhance your site, whether by increasing visitor interaction, improving discoverability, strengthening security, or maintaining site stability. [Learn more](https://experienceleague.adobe.com/en/docs/experience-manager-sites-optimizer/content/opportunity-types/overview)

### Experience Manager Assets {#aem-assets}

In AEM Assets, you can use generative AI in **Content Hub** and **AI-generated Smart Tags**.

Adobe Firefly compatibility: **Yes**

**Content Hub**

[!UICONTROL Content Hub] is available as part of [!DNL Experience Manager Assets as a Cloud Service] for democratizing access to on-brand content for organizations and their business partners. It focuses on distributing assets for activation at scale and creation of on-brand content variants for improved marketing agility.

In Content Hub, you can create content with Adobe Express (if you have Adobe Express entitlements). You can edit existing content with simple tools, produce on-brand variations with templates and brand elements, and create content with the latest GenAI capabilities from [!DNL Adobe Firefly]. [Learn more](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview)

**Smart Tags**

Instead of relying on manual input, AI can automatically assign descriptive tags to digital assets. These AI-generated tags enhance metadata quality, making the assets easier to search, categorize, and recommend. 

For example, if the asset is an image, AI can identify objects, scenes, emotions, or even brand logos. It can generate relevant tags like _sunset_, _beach_, _vacation_, or _smiling_. [Learn more](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/smart-tags#ai-smart-tags)

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO), you can use [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) to gain _product knowledge_ and _operational insights_ (beta). 

### Examples of using AI Assistant in AJO

Here's an example input for product knowledge:

* _How many live activities can I have in one Journey Optimizer sandbox?_ 

    The output is generated from Experience League and other Adobe data stores.

Here's an example input for operational insights:

* _How many Journeys have been created in the last seven days?_

    For output, AI Assistant queries a customer-specific data store. The data store contains centralized, operational data about [!UICONTROL Journeys]. This feature is customer agnostic and pulls metadata only from business objects. It does not access data within your sandbox.

[Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant)

Adobe Firefly compatibility: **No**

### AI Assistant for content generation (AJO Prime and Ultimate) {#ajo-prime}

In AJO _Prime_ and _Ultimate_, you can use [content generation](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) for content generation to bring proactive content variation suggestions for text and images.

This feature is available for email, push notifications, web page, content, and SMS channels. It provides prompt-based text and image generation. Output from content generation in AJO Prime and Ultimate is indemnified.

[Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Adobe Firefly compatibility: **Yes**

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B Edition uses [!DNL AI Assistant] to help you with product knowledge. 

Example input: 

* _How do I send an email in an account journey?_

    Product knowledge output is pulled from Experience League.

[Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Adobe Firefly compatibility: **No**

## [!DNL Campaign] Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services uses [!DNL AI Assistant] for content generation. This feature lets you auto-generate personalized, engaging, and effective content based on your marketing objective, with content optimized for brand outlined styles, layouts, tone, and more. You can use it across channels like email, SMS, and push.

**Note:** Output from content generation in Campaign Managed Cloud Services is indemnified. 

[Learn more](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Adobe Firefly compatibility: **Yes**

## [!DNL Customer Journey Analytics] {#cja}

Customer Journey Analytics lets you use generative AI in the following ways:

* [!DNL AI Assistant] for product knowledge
* [!DNL Product Support Agent] in AI Assistant
* [!UICONTROL Intelligent Captions] in Workspace visualizations
* AI and GenAI to assign every asset metadata automatically in [!DNL Content Analytics]

Adobe Firefly compatibility: **No**

**AI Assistant**

Discover product knowledge from Experience League. If you're a new user, quickly learn Customer Journey Analytics concepts and onboard yourself to products and features. For example:

* _How do I send an email in an account journey?_

Experienced users get advanced use cases or learn strategies to perform tasks at a fast pace. You can quickly understand concepts, troubleshoot problems, or search for information. 

[Learn more](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

**Intelligent Captions**

You can use _Intelligent Captions_ in [!DNL Customer Journey Analytics] to get natural-language insights for the most frequently used Workspace visualizations. Intelligent captions are ideal for analysts who need narratives and context to share with other users. Business users can use it to discover high-level takeaways quickly.

For example:

* **Input:** In CJA, run a supported visualization (including Line, Area, Bar chart, Flow, or Fallout), then click **[!UICONTROL Intelligent captions]**. 

* **Output:** View auto-generated, natural-language captions showing context and key takeaways. Then, you can take actions on the generated data, such as reviewing, copying, and sharing it with your organization. [See how](https://video.tv.adobe.com/v/3420131/?quality=12&learn=on#_blank)

[Learn more](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

**Content Analytics**

Content Analytics uses AI and GenAI to assign every asset metadata automatically, such as subjects, scenes, foreground colors, and so on. An attribute is an AI-assigned metadata tag describing what is in an asset or experience. 

For example: foreground `color: red` is an automatically assigned attribute. The visualizations help you identify which attributes of your assets contribute most to conversion. [Learn more](https://experienceleague.adobe.com/en/docs/analytics-platform/using/content-analytics/report/report#template)

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP uses [!DNL AI Assistant] to help you with product knowledge from Experience League. It also offers operational insights (in beta). [!DNL AI Assistant] queries a customer-specific operational insights data store that contains centralized operational data, partitioned in your AEP sandbox. The system pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. 

For example, if you query about an audience, [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. 

[Learn more](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)

Adobe Firefly compatibility: **No**

## [!DNL Marketo] {#marketo}

In Marketo (premium), generative AI is available in Interactive Webinars and Dynamic Chat.

**Interactive Webinars**

Automatically generate chapters and summaries for your recorded webinars, making them more accessible and easier to navigate for your audience. Features include:

* Automatic chapter generation
* AI-generated text summary
* Editable content - Modify generated chapters and summaries
* Easy integration - Add chapters and summaries to your Landing Pages by copying the HTML code to the webpage editor of your choice

[Learn more](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai)

**Dynamic Chat**

Generative AI powered capabilities in Adobe Dynamic Chat allow you to optimize productivity for your sales agents, get insights into your website visitor intent, and respond to visitor questions in a safe manner. You can pre-approve the questions, answers, and the conversation summary. 

[Learn more](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Adobe Firefly compatibility: **No**

## [!DNL Workfront] {#workfront}

[!DNL AI Assistant] in [!DNL Workfront] helps you accomplish your work by offering in-app information and suggestions. You can:

* Get summaries of some objects, giving you a high-level view of the object's intent or details.
* Ask questions and let [!DNL AI Assistant] find answers on Experience League.
* Get generated formulas based on your prompts. You can also resolve errors in your invalid custom expressions in calculated fields.
* Locate projects, tasks, and issues.

[Learn more](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Adobe Firefly compatibility: **No**

## Additional resources

* [Responsible AI Resources on Trust Center](https://www.adobe.com/trust/responsible-ai.html)<!-- * [Customer AI Propensity Scoring Model Card](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/model-cards/ai-model-cards/customer-ai) -->

**Disclaimer:** The information on this page is for general informational purposes only. We aim to keep it accurate and up to date, but software and AI features may change frequently. We do not guarantee the completeness or reliability of the information at all times. Please double-check any important details before making decisions based on this content.
