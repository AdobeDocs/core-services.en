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
# AI in Experience Cloud applications

This page helps you understand generative AI and how you can use it in Experience Cloud applications. Learn which product features use generative AI, AI Assistant, and whether Adobe Firefly is supported.

## About generative AI and AI Assistant

Generative AI is a type of artificial intelligence that does more than simply answer questions. It _creates_ content and _responds_ to your _prompts_ (questions and statements). 

* **Create:** Refers to the AI's ability to generate new content (text, images, music, or videos) from scratch, based on its training and input prompts. This ability is the _generative_ aspect of generative AI.

* **Respond:** Refers to the AI providing an answer or reaction to a specific prompt, typically drawing on its knowledge or reasoning capabilities.

If you're new to Experience Cloud, you can use generative AI to gain product knowledge quickly. As an experienced user, you can discover operational insights in seconds rather than hours.

### AI Assistant

[AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/landing) is a conversational tool supported in Experience Platform and related applications. Use it to accelerate your workflows, improve your product knowledge, troubleshoot problems, or search through information. In certain applications, AI Assistant lets you discover operational insights immediately. 

Product knowledge responses from Experience League are verifiable and cited with links. Learn about the types of [objective-based prompts](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to get the most out of AI Assistant.

<!-- **Your data remains yours**

In AI Assistant, security is the priority:

* Customer data is not used to train language models.
* AI Assistant looks at only the documents that you tell it to. You are in control.
* Your people can use AI Assistant only on documents they can access.
* It's audit-ready: Responses are attributable to source documents.
* Enterprise controls are in place to manage who has AI access in the company. -->

## Applications with features that support AI

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

### GenStudio for Performance Marketing {#gspm}

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is a generative AI-driven platform with capabilities that can transform how marketing content is created, reviewed, shared, and analyzed. 

On the [Create](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview) home, you can create high-performing, on-brand experiences. Generate content for: 

* Emails
* Meta ads
* LinkedIn ads
* Display ads
* Banners

You can also train GenStudio for Performance Marketing on your brand using examples, descriptions of customer personas and products, and brand guidelines. [Learn more...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview) 

**Compatible withe Adobe Firefly:** Planned

### Generate Variations in Experience Manager Sites {#aem-sites}

[Generate Variations](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations) in AEM Sites uses generative AI to create content variations based on prompts. These prompts are either provided by [Adobe](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) or created and managed by [users](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt). 

After creating variations, you can use the content on your website and measure its success using the Experimentation feature in Edge Delivery Services. 

### Input and output fields

Input fields include: 
 
* Number of Variations to generate
* Audience Source
* Audience Target
* Additional Context
* Customer-driven prompts 

The output is generated content or market copy. 

You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly. [Learn more...](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image)

**Compatible with Adobe Firefly:** Yes
 
## AI Assistant in Journey Optimizer {#journey-optimizer}

In Journey Optimizer, AI Assistant can help you gain product knowledge and operational insights.

**Product knowledge:** AI Assistant queries Adobe data stores (such as Experience League product documentation) for product insight. The output is customer agnostic. 

Example:

* _How many live activities can I have in one Adobe Journey Optimizer sandbox?_

**Operational Insights (Beta)** - AI Assistant queries a customer-specific operational insights data store that contains centralized operational data about Journeys, partitioned by the customer's sandbox. This feature pulls metadata only from business objects and does not access data within the sandbox.

Example prompt: 

* _How many Journeys have been created in the last seven days?_

Operational Insights output depends on metadata pulled from customer's business objects. This output is customer agnostic.

_Journeys_ is the only object available for AI Assistant in Journey Optimizer, and metadata is pulled from the current sandbox. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant).

**Compatible withe Adobe Firefly:** No

## AI Assistant in Journey Optimizer Prime and Ultimate {#ajo-prime-ultimate}

Journey Optimizer Prime and Ultimate use [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) to bring proactive content variation suggestions for text and images. 

This feature is available for [email](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email), [push notifications](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push), [web page](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web), [content](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation), and [SMS](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) channels. It provides prompt-based text and image generation. 

**Note:** Output from Content Accelerator in AJO Prime and Ultimate is indemnified.

**Compatible withe Adobe Firefly:** Yes

## AI Assistant in Journey Optimizer B2B Edition {#ajo-b2b}

Journey Optimizer B2B Edition uses [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/ai-assistant-overview) to help you with product knowledge, based on your product knowledge prompts. 

**Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. 

* **Input:** How do I send an email in an account journey?

* **Output:** Product Knowledge pulls from Experience League (public documentation). [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/ai-assistant/question-guidance)

**Compatible withe Adobe Firefly:** No

## AI Assistant in Campaign Managed Cloud Services {#campaign-cs}

Campaign Managed Cloud Services uses [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs). This feature lets you auto-generate personalized, engaging, and effective content based on your marketing objective, with content optimized for brand outlined styles, layouts, tone, and more. You can use it across channels like [email](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content), [SMS](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms), and [push](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push). 

**Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. 

**Compatible withe Adobe Firefly:** Yes

## AI Assistant in Customer Journey Analytics {#cja}

Customer Journey Analytics uses [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/ai-assistant) to help you discover product knowledge and insights from Experience League. 

**Example prompt:** How do I build a calculated metric? 

New users can use it to learn Customer Journey Analytics concepts and onboard yourself to products and features that you are unfamiliar with. 

Experienced users can use AI Assistant to present more advanced use cases or tips and tricks and perform tasks at a fast pace. Understand concepts, troubleshoot problems, or search for information. [Learn more...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) 

**Compatible withe Adobe Firefly:** No

## Intelligent Captions in Customer Journey Analytics {#cja-captions}

[Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) in Customer Journey Analytics provide natural-language insights for the most frequently used Workspace visualizations.

**Compatible withe Adobe Firefly:** No

## AI Assistant in Real-Time CDP {#rtcdp}

Real-Time CDP uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to help you discover product knowledge and insights from Experience League. [Get tips](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/questions) on asking questions.

It also offers operational insights (in beta). AI Assistant queries a customer-specific operational insights data store that contains centralized operational data, partitioned by the customer's AEP sandbox. It pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. 

For example, for a query about an audience, [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. 

For example: 

* Input: _How many datasets do I have?_ 

* Response: Operational Insights output depends on metadata pulled from Customer's business objects (Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources), and includes a link to specific UI page containing queried data.

For more examples, see the _Product Knowledge_ and _Operational Insights_ input tables in [AI Assistant in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)  

**Compatible with Firefly:** No

## Dynamic Chat in Marketo {#marketo}

Generative AI powered capabilities in Adobe Dynamic Chat allow you to optimize productivity for your sales agents, get insights into your website visitor intent, and respond to visitor questions in a safe manner. You can pre-approve the questions, answers, and the conversation summary. [Learn more...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/overview)

**Compatible with Firefly:** No

## AI Assistant in Workfront {#workfront}

AI Assistant in Workfront helps you accomplish your work by offering in-app information and suggestions. You can:

* Get summaries of some objects, giving you a high-level view of the object's intent or details.
* Ask questions and let [!DNL AI Assistant] find answers on Experience League.
* Get generated formulas based on your prompts. You can also resolve errors in your invalid custom expressions in calculated fields.
* Locate projects, tasks, and issues.

[Learn more...](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview)

**Compatible with Firefly:** No
