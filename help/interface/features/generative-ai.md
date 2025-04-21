---
title: AI in Experience Cloud applications
description: Learn how Experience Cloud applications use generative AI and AI Assistant.
solution: Experience Cloud
feature: AI Assistant, Generative AI
topic: Administration
role: Admin
level: Intermediate
hide: no
hidefromtoc: yes
index: n
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

[GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is a generative AI-driven platform that enables you to you create, deliver, and optimize campaign assets. Its generative AI capabilities transform how marketing content is created, reviewed, shared, and analyzed.

The feature _GenStudio for Performance Marketing Create_ (or, simply _Create_) allows marketers and distributed teams to create high-performing, on-brand experiences. You can generate content for: 

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

**Input:** Input fields include: 
 
* Number of Variations to generate
* Audience Source
* Audience Target
* Additional Context
* Customer-driven prompts 

**Output:** Generated Content / Market Copy. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly. 
 
See [Generate Image](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image) to learn more.

**Compatible with Adobe Firefly:** Yes
 
## AI Assistant in Journey Optimizer {#journey-optimizer}

In Journey Optimizer, AI Assistant can help you gain product knowledge and operational insights.

**Product knowledge:** AI Assistant queries Adobe data stores (such as Experience League product documentation) for product insight. The output is customer agnostic. 

Example:

* _How many live activities can I have in one Adobe Journey Optimizer sandbox?_

**Operational Insights (Beta)** - Queries a customer-specific operational insights data store that contains centralized operational data about Journeys, partitioned by the customer's sandbox. This feature pulls metadata only from business objects and does not access data within the sandbox.

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

Campaign Managed Cloud Services uses [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more across channels like [email](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content), [SMS](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms), and [push](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push). 

**Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. 

**Compatible withe Adobe Firefly:** Yes

## AI Assistant in Customer Journey Analytics {#cja}

CJA uses [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) to help you discover product knowledge and insights from Experience League. 

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

* Response: _Operational Insights output depends on metadata pulled from Customer's business objects (Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources), and includes a link to specific UI page containing queried data._

For more examples, see the _Product Knowledge_ and _Operational Insights_ input tables in [AI Assistant in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)  

**Compatible with Firefly:** No

## Dynamic Chat in Marketo {#marketo}

[Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) creates AI-assisted conversations with customized and pre-approved questions and answers, as well as conversation summary |<ul><li> **Generate Questions:** Provide URLs from which content is extracted and used to generate questions / responses. </li><li> **Conversation Summary:** Generates a summary of a chat conversation. </li></ul> [Learn more...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | No |

## AI Assistant in Workfront {#workfront}

[AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront helps you accomplish your work by offering in-app information and suggestions in a natural-language conversation. AI Assistant offers the following functionality: Summarizes projects/tasks/issues/documents, provides instructions or reference information pulled from the Workfront documentation on Experience League, generates or refines formulas for calculated custom fields.  | <ul><li>**Summarize Project Input:** Summarize this project </li><li> **Summarize Project Output:** Returns brief descriptions of the project's purpose and status, gives examples of tasks that are completed and that are still pending, and provides some additional details and notes.</li><li> **Generate/Refine Formula Input:** "Rewrite this formula to remove the invalid expression error." </li><li> **Generate/Refine Formula Output:** Generated or refined formula. </li></ul>**Note:** AI Assistant may take a few moments to generate the revised formula, depending on the size and complexity of the formula. | No  |


<!-- ## Experience Cloud applications that use AI

Learn how Experience Cloud applications use generative AI or AI Assistant, and whether Adobe Firefly is supported. 

| Application | How Generative AI Is Used | Examples | Adobe Firefly? |
|----------|------------|-----------|----------------|
| GenStudio for Performance Marketing | [GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home) is a generative AI-driven platform. It infuses the content creation lifecycle with generative AI capabilities that transform how marketing content is created, reviewed, shared, and analyzed.<br>You can train GenStudio for Performance Marketing on your brand using examples, descriptions of customer personas and products, and brand guidelines. |_GenStudio for Performance Marketing Create_ lets you generate content for emails, Meta ads, LinkedIn ads, display ads, and banners. <br>**Inputs:** <ul><li>Use templates to start the content creation process. </li><li>Add parameters like Brands, Products, and Personas (guidelines) and Content (assets) to shape the generated experience. </li><li>Enter descriptive prompts that describe the context or experience you intend to generate. [Learn more...](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/overview)</li></ul> |Yes |
|Adobe Experience Manager Sites (Cloud Service)  | AEM Sites uses [Generate Variations](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations). <br>Generate Variations uses generative AI to create content variations based on prompts. These prompts are either provided by Adobe or created and managed by users. |After creating variations, you can use the content on your website and measure its success using the Experimentation functionality of Edge Delivery Services. <br>**Input:** Input fields include Number of Variations to generate; Audience Source / Audience Target; Additional Context, and customer-driven prompts. <ul><li>[Adobe prompt template](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#get-started) </li><li>[User generated prompt](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#create-prompt)</li></ul> **Output:** Generated Content / Market Copy. You also have the option to generate images in Adobe Express using the generative AI capabilities of Firefly. See [Generate Image](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/generative-ai/generate-variations#generate-image). | Yes|
| Adobe Journey Optimizer |Journey Optimizer uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) with two classes of questions:<ul><li>**Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. </li><li>**Operational Insights (Beta)** - queries a customer-specific operational insights data store that contains centralized operational data about Journeys, partitioned by the customer's sandbox. Pulls metadata only from business objects and does not access data within the sandbox.</li></ul>|<ul><li>**Product Knowledge Input:** How many live activities can I have in one Adobe Journey Optimizer sandbox?</li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li>**Operational Insights Input:** How many Journeys have been created in the last seven days? </li><li>**Operational Insights Output:** Operational Insights output depends on metadata pulled from customer's business objects. Journeys is the only object available in AJO, and metadata is pulled from the current sandbox. </li></ul> See [Work with the AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/get-started/ai-assistant) and [Field Readiness](https://fieldreadiness-adobe.highspot.com/items/6661f1c132683fd5e6a8adf4?lfrm=srp.1#11) | No |
| Journey Optimizer: _Prime_ and _Ultimate_  | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/gs-generative) brings proactive content variation suggestions for text and images. It is available for email, push, web and SMS channels. This new capability provides prompt-based text and image generation. |<ul><li> **Email** - generate a full email, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-email) </li><li> **Push Notification** - Generate a full push notification, text only or image only. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-push) </li><li> **SMS** - Generate a full SMS, or text only. [Learn more](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-sms) </li><li> **Webpage** - Generate web page images or web page text. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-web) </li><li> **Content** - Generate content for various messaging campaigns. [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/ai-assistant/generative-experimentation)</li></ul> **Note:** Output from Content Accelerator in AJO Prime and Ultimate is indemnified. | Yes   |
| Journey Optimizer B2B Edition  | Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant) with one class of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. | <ul><li>**Input:** How do I send an email in an account journey?</li><li>**Output:** Product Knowledge pulls from Experience League (public documentation). [Learn more...](https://experienceleague.adobe.com/en/docs/journey-optimizer-b2b/user/get-started/ai-assistant)</li></ul>   | No   |
| Campaign Managed Cloud Services | [AI Assistant for Content Accelerator](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-gs) auto-generates personalized, engaging, and effective content based on the marketing objective with content optimized for brand outlined styles, layouts, tone, and more across channels like Email, SMS, Push. |<ul><li> **Email** - Generate a full email, text only or image only. [Learn more](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-content) </li><li> **SMS** - Generate full SMS or text only. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-sms) </li><li> **Push** - Craft compelling messaging and generate content. [Learn more...](https://experienceleague.adobe.com/en/docs/campaign-web/v8/content/ai-assistant/generative-push) </li></ul> **Note:** Output from Content Accelerator in Campaign Managed Cloud Services is indemnified. | Yes  |
| Customer Journey Analytics   | CJA uses [AI Assistant](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant) to help you discover product knowledge and insights from Experience League. <br>For example, new users can use it to learn Customer Journey Analytics concepts and onboard yourself to products and features that you are unfamiliar with. <br>Experienced users can use AI Assistant to present more advanced use cases or tips and tricks and perform tasks at a fast pace. Understand concepts, troubleshoot problems, or search for information. [Learn more...](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/ai-assistant#knowledge) | <ul><li>**Product Knowledge Input:** How do I build a calculated metric? </li><li> **Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li></ul> | No |
| Customer Journey Analytics    | [Intelligent Captions](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/visualizations/intelligent-captions) provides natural-language insights for line visualizations in Workspace visualizations.| <ul><li>**Input:** Line visualizations. Captions are auto-generated based on such line visualizations when you click **Intelligent captions**. </li><li> **Output:** Auto-generated natural-language captions.</li></ul>  | No             |
| Real-Time CDP |Uses [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home) to help you discover product knowledge and insights from Experience League. It queries a database and translates data from the database into a human-readable answer. Two classes of questions: <br> **Product knowledge** - Queries Adobe data stores (such as Experience League product documentation) for product insight. This output is customer agnostic. <br> **Operational Insights (Beta)** - Queries a customer-specific operational insights data store that contains centralized operational data, partitioned by the customer's AEP sandbox. Pulls metadata only from Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources, and does not access data within the sandbox. <br>For example, for a query about an audience [!DNL AI Assistant] can access the name of the audience and other associated metadata but cannot access the profiles within that audience. | <ul><li>**Product Knowledge Input:** How is profile richness calculated? </li><li>**Product Knowledge Output:** Product Knowledge pulls from Experience League (public documentation). </li><li> **Operational Insights Input:** How many datasets do I have? </li><li> **Operational Insights Output:** Operational Insights output depends on metadata pulled from Customer's business objects (Attributes, Audiences, Dataflows, Datasets, Destinations, Schemas, and Sources), and includes a link to specific UI page containing queried data. </li></ul>For examples, see the _Product Knowledge_ and _Operational Insights_ input tables in [AI Assistant in Experience Platform](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/home)  | No |
| Marketo  | [Dynamic Chat](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview) creates AI-assisted conversations with customized and pre-approved questions and answers, as well as conversation summary |<ul><li> **Generate Questions:** Provide URLs from which content is extracted and used to generate questions / responses. </li><li> **Conversation Summary:** Generates a summary of a chat conversation. </li></ul> [Learn more...](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/generative-ai/response-library)  | No |
| Workfront | [AI Assistant](https://experienceleague.adobe.com/en/docs/workfront/using/basics/ai-assistant/ai-assistant-overview) in Workfront helps you accomplish your work by offering in-app information and suggestions in a natural-language conversation. AI Assistant offers the following functionality: Summarizes projects/tasks/issues/documents, provides instructions or reference information pulled from the Workfront documentation on Experience League, generates or refines formulas for calculated custom fields.  | <ul><li>**Summarize Project Input:** Summarize this project </li><li> **Summarize Project Output:** Returns brief descriptions of the project's purpose and status, gives examples of tasks that are completed and that are still pending, and provides some additional details and notes.</li><li> **Generate/Refine Formula Input:** "Rewrite this formula to remove the invalid expression error." </li><li> **Generate/Refine Formula Output:** Generated or refined formula. </li></ul>**Note:** AI Assistant may take a few moments to generate the revised formula, depending on the size and complexity of the formula. | No  | -->
