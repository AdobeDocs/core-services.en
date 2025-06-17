---
title: Generative AI in Experience Cloud Applications
description: Learn about generative AI (GenAI) and how Experience Cloud applications use GenAI and [!UICONTROL AI Assistant]. 
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Artificial Intelligence
role: Admin, User
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
---
# Generative AI in Experience Cloud products

Generative AI (genAI) in Experience Cloud helps you automate creative and cognitive tasks and enhance productivity. This page describes where Experience Cloud applications support genAI and AI Assistant, and provides links to learn more about these features.

**What is genAI?**

Generative AI is a type of AI that can create original content. For example, it can create text, images, video, audio, or software code in response to a user's prompt or request.

* **Create:** The ability to generate content (text, images, music, or videos) from scratch, based on its training and input prompts. This ability is the _generative_ aspect of generative AI.

* **Generate a response:** AI provides an answer or reaction to a prompt, typically drawing on its available data and knowledge repositories.

This type of AI contrasts with [agentic AI](agentic-ai.md) (Adobe's agentic framework), which refers to AI that operates autonomously. 

**What is [!UICONTROL AI Assistant]?**

[!UICONTROL AI Assistant] is a conversational tool supported in Experience Platform and related applications. Use it to quicktly gain _product knowledge_ and _operational insights_ in supported products.

* **Product knowledge:** Product knowledge refers to concepts and topics grounded in Experience League documentation. Learn how to create effective, [objective-based prompts](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to get the most out of [!UICONTROL AI Assistant]. All responses from Experience League are verifiable and cited with links.

* **Operational insights:** [Operational insights](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions#objects-questions) refer to generated responses about your metadata objects (attributes, audiences, dataflows, datasets, and so on). With [!UICONTROL AI Assistant], you can accomplish in seconds what otherwise might take hours or days.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing" tooltip="Go to AI Assistant"}

## AI availability in Experience Cloud products

Here's a roundup of the Experience Cloud applications that use GenAI, AI Assistant, or agentic AI. Compatibility with Adobe Firefly is indicated.

| **Product Name** | **Generative AI** | **AI Assistant** | **Firefly Compatibility** |
|------------------|-------------------------|------------------|---------------------------|
| [Adobe GenStudio for Performance Marketing](#gspm) | Yes. <br> Helps marketing and creative teams create personalized, on-brand content. | Not applicable | Yes |
| [Adobe Experience Manager Sites](#aem) | Yes. <br> Available in [Generate Variations](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor?lang=en) to create content variations based on input. | Not applicable | Yes |
| [Sites Optimizer](#aem) | Yes. <br> Helps you analyze and improve the performance and effectiveness of web experiences. | Not applicable | No |
| [Adobe Experience Manager Assets](#aem) | Yes. <br>  Available in [Content Hub](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview?lang=en) and AI-generated [Smart Tags](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/smart-tags?lang=en#ai-smart-tags). | Not applicable | Yes |
| [Adobe Journey Optimizer](#journey-optimizer) | Not applicable  |Yes. <br>  Available for product knowledge and operational insights. | No |
| | |AJO Prime and Ultimate offer [Content generation](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative?lang=en) to bring proactive content variation suggestions for text and images. | Yes |
| [[!DNL Adobe Journey Optimizer] B2B Edition](#ajo-b2b) | Not applicable | Yes. <br>Available to help with product knowledge. | No |
| [[!DNL Campaign] Managed Cloud Services](#campaign-cs) | Not applicable | Yes. <br>Uses AI Assistant for Content Accelerator to auto-generate personalized, engaging, and effective content based on marketing objectives across channels like Email, SMS, and Push | Yes |
| [[!DNL Customer Journey Analytics]](#cja) |Yes. <br> GenAI is used in:<ul><li> [Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions?lang=en): For insights about the most frequently used Workspace visualizations.</li><li>[Content Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/content-analytics/report/report?lang=en#template): To assign asset metadata automatically.</li></ul> |Yes. <br>AI Assistant can help with:<ul><li>[Product knowledge](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant?lang=en) (Experience League)</li><li>[Product Support Agent](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/new-features/customer-support?lang=en) </li><li>[Data Insights Agent](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai)</li></ul> | No |
| [[!DNL Real-Time CDP]](#rtcdp) | Not applicable | Yes. <br>Product knowledge from Experience League. It also offers operational insights (in beta).| No |
| [[!DNL Marketo]](#marketo) |Yes. <br>Available in [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview?lang=en) and [Interactive Webinars](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai?lang=en). | Not applicable | No |
| [[!DNL Workfront]](#workfront) |Yes. <br> In-app information and suggestions. [Learn more](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview?lang=en)| Not applicable | Yes |

## Examples of using GenAI in Experience Cloud {#products}

The following sections go into more detail about how you can use genAI or AI Assistant in specific applications. Links to learn more are provided.

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

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home" tooltip="Go to GenStudio for Performance Marketing"}

<!-- [Learn more](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) -->

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

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations-integrated-editor" tooltip="Go to Generate Variations on Experience League"}

### Sites Optimizer {#sites-optimizer}

AEM Sites Optimizer uses generative AI to analyze and improve the performance and effectiveness of web experiences. These insights are grouped into key opportunity areas: Engagement, Traffic Acquisition, Security Posture, and, Site Health. Each category highlights specific ways to enhance your site, whether by increasing visitor interaction, improving discoverability, strengthening security, or maintaining site stability.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/experience-manager-sites-optimizer/content/opportunity-types/overview" tooltip="Go to Sites Optimizer on Experience League"}

### Experience Manager Assets {#aem-assets}

In AEM Assets, you can use generative AI in **Content Hub** and **AI-generated Smart Tags**.

**Content Hub**

[!UICONTROL Content Hub] is available as part of [!DNL Experience Manager Assets as a Cloud Service] for democratizing access to on-brand content for organizations and their business partners. It focuses on distributing assets for activation at scale and creation of on-brand content variants for improved marketing agility.

In Content Hub, you can create content with Adobe Express (if you have Adobe Express entitlements). You can edit existing content with simple tools, produce on-brand variations with templates and brand elements, and create content with the latest GenAI capabilities from [!DNL Adobe Firefly]. 

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview" tooltip="Go to Content Hub on Experience League"}

**Smart Tags**

Instead of relying on manual input, AI can automatically assign descriptive tags to digital assets. These AI-generated tags enhance metadata quality, making the assets easier to search, categorize, and recommend. 

For example, if the asset is an image, AI can identify objects, scenes, emotions, or even brand logos. It can generate relevant tags like _sunset_, _beach_, _vacation_, or _smiling_. 

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/smart-tags#ai-smart-tags" tooltip="Learn about Smart Tags"}

## Adobe [!DNL Journey Optimizer] {#journey-optimizer}

In [!DNL Journey Optimizer] (AJO), you can use [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) to gain _product knowledge_ and _operational insights_ (beta). 

### Examples of using AI Assistant in AJO

Here's an example input for product knowledge:

* _How many live activities can I have in one Journey Optimizer sandbox?_ 

    The output is generated from Experience League and other Adobe data stores.

Here's an example input for operational insights:

* _How many Journeys have been created in the last seven days?_

    For output, AI Assistant queries a customer-specific data store. The data store contains centralized, operational data about [!UICONTROL Journeys]. This feature is customer agnostic and pulls metadata only from business objects. It does not access data within your sandbox.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant" tooltip="Learn about AI Assistant in AJO"}

### AI Assistant for content generation (AJO Prime and Ultimate) {#ajo-prime}

In AJO _Prime_ and _Ultimate_, you can use [content generation](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) for content generation to bring proactive content variation suggestions for text and images.

This feature is available for email, push notifications, web page, content, and SMS channels. It provides prompt-based text and image generation. Output from content generation in AJO Prime and Ultimate is indemnified.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative" tooltip="Learn about AI Assistant in AJO"}

## [!DNL Journey Optimizer B2B Edition] {#ajo-b2b}

Journey Optimizer B2B Edition uses [!UICONTROL AI Assistant] to help you with product knowledge. 

Example input: 

* _How do I send an email in an account journey?_

    Product knowledge output is pulled from Experience League.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview" tooltip="Learn about AI Assistant in AJO"}

## [!DNL Campaign] Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services uses [!UICONTROL AI Assistant] for content generation. This feature lets you auto-generate personalized, engaging, and effective content based on your marketing objective, with content optimized for brand outlined styles, layouts, tone, and more. You can use it across channels like email, SMS, and push.

**Note:** Output from content generation in Campaign Managed Cloud Services is indemnified. 

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs" tooltip="Learn about AI Assistant in AJO"}

## [!DNL Customer Journey Analytics] {#cja}

Customer Journey Analytics lets you use generative AI or AI Assistant in the following ways:

* [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) for product knowledge.
* [Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) to provide key insights for the most frequently used Workspace visualizations in natural language.
* [Content Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/content-analytics/report/report#template) to assign every asset metadata automatically.

**AI Assistant**

Discover product knowledge from Experience League. If you're a new user, quickly learn Customer Journey Analytics concepts and onboard yourself to products and features. For example:

* _How do I send an email in an account journey?_

Experienced users get advanced use cases or learn strategies to perform tasks at a fast pace. You can quickly understand concepts, troubleshoot problems, or search for information. 

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant" tooltip="Learn about AI Assistant in CJA"}

**Intelligent Captions**

You can use _Intelligent Captions_ in [!DNL Customer Journey Analytics] to get natural-language insights for the most frequently used Workspace visualizations. Intelligent captions are ideal for analysts who need narratives and context to share with other users. Business users can use it to discover high-level takeaways quickly.

For example:

* **Input:** In CJA, run a supported visualization (including Line, Area, Bar chart, Flow, or Fallout), then click **[!UICONTROL Intelligent captions]**. 

* **Output:** View auto-generated, natural-language captions showing context and key takeaways. Then, you can take actions on the generated data, such as reviewing, copying, and sharing it with your organization. [See how](https://video.tv.adobe.com/v/3420131/?quality=12&learn=on#_blank)

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions" tooltip="Learn about Intelligent Captions"}

**Content Analytics**

Content Analytics uses AI and GenAI to assign every asset metadata automatically, such as subjects, scenes, foreground colors, and so on. An attribute is an AI-assigned metadata tag describing what is in an asset or experience. 

For example: foreground `color: red` is an automatically assigned attribute. The visualizations help you identify which attributes of your assets contribute most to conversion. 

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/analytics-platform/using/content-analytics/report/report#template" tooltip="Learn about Content Analytics"}

## [!DNL Real-Time CDP] {#rtcdp}

Real-Time CDP uses [!UICONTROL AI Assistant] to help you with product knowledge from Experience League. It also offers operational insights (in beta). [!UICONTROL AI Assistant] queries a customer-specific operational insights data store that contains centralized operational data, partitioned in your AEP sandbox. The system pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. 

For example, if you query about an audience, [!UICONTROL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. 

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home" tooltip="Learn about Real-Time CDP"}

## [!DNL Marketo] {#marketo}

In Marketo, generative AI is available in Interactive Webinars and Dynamic Chat.

**Interactive Webinars**

Automatically generate chapters and summaries for your recorded webinars, making them more accessible and easier to navigate for your audience. Features include:

* Automatic chapter generation
* AI-generated text summary
* Editable content - Modify generated chapters and summaries
* Easy integration - Add chapters and summaries to your Landing Pages by copying the HTML code to the webpage editor of your choice

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai" tooltip="Learn about Interactive Webinars"}

**Dynamic Chat**

Generative AI powered capabilities in Adobe Dynamic Chat allow you to optimize productivity for your sales agents, get insights into your website visitor intent, and respond to visitor questions in a safe manner. You can pre-approve the questions, answers, and the conversation summary. Dynamic Chat includes both a free and premium version.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview" tooltip="Learn about Dynamic Chat"}

## [!DNL Workfront] {#workfront}

[!UICONTROL AI Assistant] in [!DNL Workfront] helps you accomplish your work by offering in-app information and suggestions. You can:

* Get summaries of some objects, giving you a high-level view of the object's intent or details.
* Ask questions and let [!UICONTROL AI Assistant] find answers on Experience League.
* Get generated formulas based on your prompts. You can also resolve errors in your invalid custom expressions in calculated fields.
* Locate projects, tasks, and issues.

[!BADGE Learn more]{type=Informative url="https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview" tooltip="Learn about AI Assistant in Workfront"}

## Additional resources

* [Responsible AI Resources on Trust Center](https://www.adobe.com/trust/responsible-ai.html)<!-- * [Customer AI Propensity Scoring Model Card](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/model-cards/ai-model-cards/customer-ai) -->

**Disclaimer:** The information on this page is for general informational purposes only. While effort is made to ensure the information remains accurate and current, software and generative AI features may change frequently. Accordingly, we do not warrant the completeness, accuracy, or reliability of the information at all times. Please verify any important details before making decisions based on this content.

