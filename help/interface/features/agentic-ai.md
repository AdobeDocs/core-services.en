---
title: Agentic AI in Experience Cloud Applications
description: Learn where agentic AI is available in Experience Cloud applications.
solution: Experience Cloud
landing-page-name: ai
landing-page-breadcrumb-title: AI Documentation
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
hidefromtoc: yes
index: no
exl-id: c1a8f9a7-4752-4040-b5f0-dc775417f536
---
# Agentic AI in Adobe Experience Cloud

Updated: **January 29, 2026**

Adobe Experience Platform agents use the Experience Platform [Agent Orchestrator](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home) to add agent-based capabilities to Experience Cloud applications.

These agents help automate tasks, deliver insights faster, and streamline workflows. As a result, teams can work more efficiently and get more value from Experience Cloud.

Access to AI agents in Experience Cloud is available in either:

* [Existing Experience Cloud applications](#existing-apps)
* [AI-first Experience Cloud applications](#ai-first-apps)

The following sections describe how you can enable agentic AI in Experience Cloud.

## Existing Experience Cloud applications {#existing-apps}

In existing applications, you can use natural language to instruct Adobe Experience Platform Agents through the [AI Assistant](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/home) conversational interface. The AI Assistant is available in both full-screen and right-rail views.

Agents can be enabled in existing Experience Cloud apps for customers in one of the following categories:

* Purchased an Adobe Experience Platform Agents AI Credits license
* Are included in a usage-bound trial (limited AI Credits provided)
* Transacted the Agent Orchestrator Promo SKU (time-bound trial license)

As you use AI agents to perform _agent jobs_, you consume AI credits. Learn about it in [Agent jobs and AI credit consumption](/help/interface/features/ai-credit-consumption.md).

AI agents follow _your_ input, oversight, and they respect product-level access controls. You can only perform jobs or access data that you are authorized to use in the underlying Experience Cloud product.

### AI agents in existing Experience Cloud apps {#existing-apps-table}

The following table lists Experience Platform Agents available in existing Experience Cloud applications. 

| Agent name  | Capabilities | Supported applications |
|---|----------|----------|
| [Audience Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/audience)  | Empower your teams to create, manage, and optimize audiences using natural language prompts for greater ease, efficiency, and speed to market. |<ul><li>Real-Time CDP (B2B, B2C, and B2P editions)</li><li>Adobe Journey Optimizer (B2B and B2C editions)</li></ul> |
| **Content Advisor Agent** |<ul><li>[Content Discovery](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/discovery/overview): Speed authoring and boost discovery with simplified natural-language prompts to instantly find and surface Experience Manager content across images, videos, text-based documents, content fragments, and forms.</li><li>[Content Optimization](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/content-optimization/overview): Simplify creating visual content variants from source assets using natural language prompts.</li><li>[Experience Production](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/production/overview): Automates high-effort and high-volume tasks in the CMS. This agent turns manual, lengthy processes into fast, AI-assisted workflows that keep every experience current and consistent, helping your business achieve your goals.</li></ul> |<ul><li>Adobe Experience Manager (Content Discovery)</li></ul><ul><li>Adobe Experience Manager with Dynamic Media with OpenAPI (Content Optimization)</li></ul><ul><li>Adobe Experience Manager Cloud Services and Edge Delivery Services (Experience Production) </li></ul>  |
| [Data Insights Agent](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-b2c-overview/data-analysis-ai)  |  Quickly answers questions about your data. It builds relevant visualizations in Analysis Workspace using components from your data view and using your actual data. | <ul><li>Customer Journey Analytics (B2B and B2C Editions)</li></ul>  |
| **Brand Experience Agent**  |  [Deployment Support](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/development/overview): Helps AEM CS developers and technical administrators troubleshoot build-step failures in the Cloud Manager pipeline by analyzing the root cause and suggesting fixes.|  <ul><li>AI Assistant in AEM Cloud Service and Adobe Managed Services</li></ul>  |
| **Brand Governance Agent***  |[Brand Governance](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/governance/overview): Safeguard brand integrity and compliance by enforcing security, regulatory, and brand policies across Experience Manager. This agent applies brand governance to maintain visual and messaging standards. It uses granular permissions to manage access and content changes, and incorporates DRM to uphold licensing and usage constraints.|  <ul><li>Adobe Experience Manager Sites</li><li>Adobe Experience Manager Assets</li><li>Adobe Experience Manager Forms</li></ul>  |
| [Journey Agent](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/ajo-agent-analyze) | Enable your teams to quickly create, analyze, and optimize multi-touch customer journeys at scale. | <ul><li>Adobe Journey Optimizer (B2B and B2C editions)</li></ul> |
| [Product Support Agent](https://experienceleague.adobe.com/en/docs/experience-platform/ai-assistant/new-features/customer-support) |  Troubleshoot support issues without leaving your workflows, create customer support tickets, and track case progress using AI Assistant. | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2B and B2C Editions)</li><li>Adobe Journey Optimizer B2B Edition</li><li>Customer Journey Analytics</li><li>Adobe Experience Manager</li></ul>  |

Asterisk (*): This Agent is accessible to customers in the Explorer Program. The Explorer Program is an invite-only program that provides early access to Adobe's latest agentic capabilities. Please reach out to your account representative for more information. 

## AI-first Experience Cloud applications {#ai-first-apps}

AI-first applications are built with generative or agentic Al at the core. They use generative or agentic Al for key tasks, and the agentic features are already included in the Al-first application license. As such, they do not require the Experience Platform Agent Orchestrator license.

The following table lists Experience Platform Agents available as Al-first applications. They are enabled by licensing these Al-first applications:  

| Agent name  | Capabilities | Supported applications   |
|---|----------|----------|
| [Experimentation Agent](https://experienceleague.adobe.com/en/docs/journey-optimizer/using/content-management/content-experiment/experiment/experiment-accelerator-security) |  Automate, analyze, and synthesize insights, so you can quickly identify high-impact experiments and growth opportunities from a centralized workspace — all while reducing manual processes.  | <ul><li>AJO Experimentation Accelerator</li></ul>   |
| [LLM Optimization Agent](https://experienceleague.adobe.com/en/docs/llm-optimizer/using/home) |  Enhance visibility, accuracy, and influence in AI-driven search environments, provide insights into brand presence in AI-generated answers, offer prescriptive content recommendations, and automate optimization fixes. | <ul><li>Adobe LLM Optimizer</li></ul>   |
| [Site Optimization Agent](https://experienceleague.adobe.com/en/docs/experience-manager-sites-optimizer/content/home) | Maximize business impact by automatically detecting and deploying website enhancements. Using generative AI and multiple monitoring technologies, you can increase site traffic acquisition, engagement, and more | <ul><li>AEM Sites Optimizer</li></ul> |
| [Product Advisor Agent](https://experienceleague.adobe.com/en/docs/brand-concierge/content/documentation/overview) |  Boost conversion and engagement through intelligent, context-aware product discovery tailored to individual preferences and behaviors. | <ul><li>Adobe Brand Concierge</li></ul> |

## More help on this topic

* [AI in Experience Cloud](https://experienceleague.adobe.com/en/docs/ai) documentation home
* [Overview of Agents in AEM](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/ai-in-aem/agents/overview)

[!BADGE Learn more on Adobe for Business]{type=Informative url="https://business.adobe.com/products/experience-platform/agent-orchestrator.html" tooltip="Go to Business.adobe.com"}
