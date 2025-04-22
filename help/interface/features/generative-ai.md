---
title: AI in Experience Cloud applications
description: Learn about generative AI and how Experience Cloud applications use genAI and AI Assistant. 
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
exl-id: bdc51956-82aa-4aae-b627-a2018f80b5f5
---
# AI in Experience Cloud products

Generative AI is a type of artificial intelligence that does more than simply answer questions. It _creates_ content and _responds_ to your _prompts_ (questions and statements). 

* **Create:** Refers to the AI's ability to generate new content (text, images, music, or videos) from scratch, based on its training and input prompts. This ability is the _generative_ aspect of generative AI.

* **Respond:** Refers to the AI providing an answer or reaction to a specific prompt, typically drawing on its knowledge or reasoning capabilities.

If you're new to Experience Cloud, you can use generative AI to gain product knowledge quickly. As an experienced user, you can discover operational insights in seconds rather than hours.

**About AI Assistant**

AI Assistant is a conversational tool supported in Experience Platform and related applications. Use it to accelerate your workflows, improve your product knowledge, troubleshoot problems, or search through information. In certain applications, AI Assistant lets you discover operational insights immediately. 

Product knowledge responses from Experience League are verifiable and cited with links. Learn about the types of [objective-based prompts](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to get the most out of AI Assistant.

[Learn more](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) 

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company. -->

## AI availability in Experience Cloud products

Learn about support for generative AI or AI Assistant in Experience Cloud products, and whether Adobe Firefly is supported.

* [GenStudio for Performance Marketing](#gspm)
* [Generate Variations in AEM Sites (Cloud Service)](#aem-sites)
* [AI Assistant in Journey Optimizer](#journey-optimizer)
* [Adobe Journey Optimizer Prime and Ultimate](#ajo-prime-ultimate)
* [Journey Optimizer B2B Edition](#ajo-b2b)
* [AI Assistant in Journey Optimizer Prime and Ultimate](#ajo-prime-ultimate)
* [AI Assistant in Journey Optimizer B2B Edition](#ajo-b2b)
* [AI Assistant in Campaign Managed Cloud Services](#campaign-cs)
* [AI Assistant in Customer Journey Analytics](#cja)
* [Intelligent Captions in Customer Journey Analytics](#cja-captions)
* [AI Assistant in Real-Time CDP](#rtcdp)
* [Dynamic Chat in Marketo](#marketo)
* [AI Assistant in Workfront](#workfront)

## GenStudio for Performance Marketing {#gspm}

GenStudio for Performance Marketing is an AI-driven platform that empowers you to generate and manage marketing content that adheres to your brand standards and complies with your enterprise policies. Generate content for emails, Meta ads, LinkedIn ads, display ads, and banners.

You can also train GenStudio for Performance Marketing on your brand using examples, descriptions of customer personas and products, and brand guidelines. 

[Learn more](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)

Compatibility with Adobe Firefly: **Planned**

## Generate Variations in Experience Manager Sites {#aem-sites}

Generate Variations in AEM Sites uses generative AI to create content variations based on prompts. These prompts are either provided by Adobe or created and managed by you. 

After creating variations, you can use the content on your website and measure its success using the Experimentation feature in Edge Delivery Services. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly.

[Learn more](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations)

Compatibility with Adobe Firefly: **Yes**
 
## AI Assistant in Journey Optimizer {#journey-optimizer}

In Journey Optimizer, use AI Assistant to gain product knowledge and operational insights. For example, ask _How many live activities can I have in one Journey Optimizer sandbox?_ You'll immediately get your answer from Experience League and other Adobe data stores.

AI Assistant also helps with operational insights (beta). For example, you can quickly learn how many Journeys have been created in the last seven days. 

For operational insights, AI Assistant queries a customer-specific data store. The data store contains centralized, operational data about [!UICONTROL Journeys]. This feature is customer agnostic and pulls metadata only from business objects. It does not access data within your sandbox.

[Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

Compatibility with Adobe Firefly: **No**

## AI Assistant in Journey Optimizer Prime and Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime and Ultimate use AI Assistant for Content Accelerator to bring proactive content variation suggestions for text and images. 

This feature is available for email, push notifications, web page, content, and SMS channels. It provides prompt-based text and image generation. Output from Content Accelerator in AJO Prime and Ultimate is indemnified.

[Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative)

Compatibility with Adobe Firefly: **Yes**

## AI Assistant in Journey Optimizer B2B Edition {#ajo-b2b}

Journey Optimizer B2B Edition uses AI Assistant to help you with product knowledge. 

[Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview)

Compatibility with Adobe Firefly: **No**

## AI Assistant in Campaign Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services uses AI Assistant for Content Accelerator. This feature lets you auto-generate personalized, engaging, and effective content based on your marketing objective, with content optimized for brand outlined styles, layouts, tone, and more. You can use it across channels like email, SMS, and push.

**Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. 

[Learn more](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs)

Compatibility with Adobe Firefly: **Yes**

## AI Assistant in Customer Journey Analytics {#cja}

Customer Journey Analytics uses AI Assistant to help you discover product knowledge and insights from Experience League. If you're a new user, quickly learn Customer Journey Analytics concepts and onboard yourself to products and features. 

Experienced users get advanced use cases or learn strategies to perform tasks at a fast pace. Understand concepts, troubleshoot problems, or search for information. 

[Learn more](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant)

Compatibility with Adobe Firefly: **No**

## Intelligent Captions in Customer Journey Analytics {#cja-captions}

Intelligent Captions in Customer Journey Analytics provide natural-language insights for the most frequently used Workspace visualizations. Intelligent captions are ideal for analysts who need narratives and context to share with other users. Business users can use it to discover high-level takeaways quickly.

[Learn more](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions)

Compatibility with Adobe Firefly: **No**

## AI Assistant in Real-Time CDP {#rtcdp}

Real-Time CDP uses AI Assistant to help you with product knowledge from Experience League. It also offers operational insights (in beta). AI Assistant queries a customer-specific operational insights data store that contains centralized operational data, partitioned in your AEP sandbox. The system pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. 

For example, if you query about an audience, [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. 

[Learn more](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)

Compatibility with Adobe Firefly: **No**

## Dynamic Chat in Marketo {#marketo}

Generative AI powered capabilities in Adobe Dynamic Chat allow you to optimize productivity for your sales agents, get insights into your website visitor intent, and respond to visitor questions in a safe manner. You can pre-approve the questions, answers, and the conversation summary. 

[Learn more](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

Compatibility with Adobe Firefly: **No**

## AI Assistant in Workfront {#workfront}

AI Assistant in Workfront helps you accomplish your work by offering in-app information and suggestions. You can:

* Get summaries of some objects, giving you a high-level view of the object's intent or details.
* Ask questions and let [!DNL AI Assistant] find answers on Experience League.
* Get generated formulas based on your prompts. You can also resolve errors in your invalid custom expressions in calculated fields.
* Locate projects, tasks, and issues.

[Learn more](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

Compatibility with Adobe Firefly: **No**
