---
title: Agent Jobs and AI Credit Consumption
description: Learn about agent jobs and AI credit consumption rates in Experience Cloud applications.
solution: Experience Cloud
topic: Artificial Intelligence
feature: Agentic AI, AI Tools
role: Admin, User
level: Intermediate
---
# Adobe Experience Platform agent jobs and AI credits consumption  

Learn about agentic AI jobs and AI credit consumption in Experience Cloud applications. For information about enabling agentic AI capabilities in existing Experience Cloud applications, see [Agentic AI in Experience Cloud](agentic-ai.md#existing-apps).

## Agent jobs

An _agent job_ is a series of tasks and actions an agent executes to achieve a specific outcome, as directed by customer inputs.

Using natural language prompts via AI Assistant, you can ask agents to carry out specific jobs. Based on those inputs, Agent Orchestrator coordinates the appropriate agents to execute each step within the relevant Experience Cloud applications.

## AI credits

An _AI credit_ is a usage-based metric that quantifies the execution of agent jobs. AI credits do not apply to [AI-first applications](/help/interface/features/agentic-ai.md).

## AI credit consumption

AI credit usage may vary depending on the complexity and value of the job executed:

* Simple (often single-step) tasks consume fewer credits  
* Complex (often multi-step) tasks consume more credits  
* Tasks involving advanced reasoning, validation, multi-agent coordination, or integration consume more credits  

### Estimated AI credit consumption rates

| Agent | Job | Supported applications | Estimated AI credits |
|------|-----|------------------------|----------------------|
| Audience Agent | Audience/account ideation | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 50 |
| Audience Agent | Knowledge-based audience/account creation | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 150 |
| Audience Agent | Audience/account management | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience Agent | Audience/account analysis | <ul><li>Real-Time CDP</li><li>Adobe Journey Optimizer</li></ul> | 25 |
| Audience Agent | Buying group ideation | <ul><li>Adobe Journey Optimizer (B2B)</li></ul> | 25 |
| Data Insights Agent | Data analysis and visualization | <ul><li>Customer Journey Analytics (B2C and B2B Editions)</li></ul> | 25 |
| Journey Agent | Journey ideation | <ul><li>Adobe Journey Optimizer (B2B Edition)</li></ul> | 25 |
| Journey Agent | Journey creation | <ul><li>Adobe Journey Optimizer (B2B and B2C Editions)</li></ul> | 30 |
| Journey Agent | Journey analysis | <ul><li>Adobe Journey Optimizer (B2B and B2C Editions)</li></ul> | 50 |
| Journey Agent | Journey management | <ul><li>Adobe Journey Optimizer (B2B and B2C Editions)</li></ul> | 25 |
| Product Support Agent | Knowledge-based troubleshooting | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2C and B2B Editions)</li><li>Customer Journey Analytics (B2C and B2B Editions)</li></ul> | 0 |
| Product Support Agent | Support case creation and tracking | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li>Adobe Journey Optimizer (B2C and B2B Editions)<li>Customer Journey Analytics (B2C and B2B Editions)</li><li>Adobe Experience Manager</li></ul> | 10 |
| Content Advisor Agent | Content discovery | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 |
| Content Advisor Agent |  <ul><li>Content update</li><li>Content optimization</li><li>Forms creation</li> | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 10 |
| Brand Experience Agent | Deployment support | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 |
| Brand Experience Agent | Site modernization | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 100 |

>[!NOTE]
>
>Actual AI credit consumption may vary depending on the number of steps executed and iterations per step.

## More help on this topic

* [Agentic AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Adobe Experience Platform Agents usage-bound trial](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)