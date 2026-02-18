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

### Estimated AI credit consumption rates - table 1

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
| Brand Experience Agent | <ul><li>Experience Support</li><li>Deployment support</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 |
| Brand Experience Agent | Site modernization | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 100 |

### Estimated AI credit consumption rates - table 2

| Agent | Jobs | Supported application(s) | Estimated AI Credit Consumption Rate* | Sample prompts |
|------|------|--------------------------|---------------------------------------|----------------|
| **Audience Agent** | Audience / Account ideation | Real-Time CDP (B2B, B2C, and B2P Editions)<br>Adobe Journey Optimizer (B2C Edition) | **50** | <ul><li>Show me fields for affluent buyers</li><li>Find all fields related to customer preferences</li></ul> |
| **Audience Agent** | Knowledge-based Audience / Account creation | Real-Time CDP (B2B, B2C, and B2P Editions)<br>Adobe Journey Optimizer (B2C Edition) | **150** | <ul><li>Create an audience made up of people who live in California</li><li>Generate an audience of VIP members who spent over $1000 this quarter</li><li>Build an audience of users who bought clothing items but haven't made a purchase in the last 60 days</li></ul> |
| **Audience Agent** | Audience / Account management | Real-Time CDP (B2B, B2C, and B2P Editions)<br>Adobe Journey Optimizer (B2C Edition) | **25** | <ul><li>Do I have any duplicate audiences?</li><li>Show me my 5 largest audiences.</li><li>Show me audiences that are not activated to any destination</li><li>List all audiences used in live journeys</li></ul> |
| **Audience Agent** | Audience / Account analysis | Real-Time CDP (B2B, B2C, and B2P Editions)<br>Adobe Journey Optimizer (B2C Edition) | **25** | <ul><li>Which audiences have increased in size by more than 20% in the last week?</li><li>How much has audience "Loyal Platinum" changed compared to the value 30 days ago?</li><li>What is my fastest growing audience?</li></ul> |
| **Audience Agent** | Buying group ideation | Adobe Journey Optimizer (B2B Edition) | **25** | <ul><li>Which accounts are showing intent for these products?</li><li>Show me the top persons by product intent for XYZ.</li><li>Which buying groups have more than 5 members?</li></ul> |
| **Data Insights Agent** | Data analysis and visualization | Customer Journey Analytics (B2C and B2B Editions) | **25** | <ul><li>Trend orders in July</li><li>Show revenue by region.</li><li>Show orders by gender, from March to June.</li><li>What were my top 10 SKUs by profit in June</li><li>Proportion of purchases by month of year</li><li>Share of revenue by product category</li></ul> |
| **Journey Agent** | Journey ideation | Adobe Journey Optimizer (B2B Edition) | **25** | <ul><li>Create a journey for whitespace accounts with intent for my solution, focusing on people engaged with content on the website</li></ul> |
| **Journey Agent** | Journey creation | Adobe Journey Optimizer (B2C and B2B Editions) | **30** | <ul><li>Generate a journey to send a reminder to users who have not completed their first purchase in the last 7 days</li><li>When users complete their first purchase, send an SMS confirmation and follow-up benefits explanation via email after 3 days</li></ul> |
| **Journey Agent** | Journey analysis | Adobe Journey Optimizer (B2C and B2B Editions) | **50** | <ul><li>I want to analyze the fallout by node for journey Fourth of July Campaign.</li><li>Are there any scheduling conflicts for journey X</li><li>Show me audience overlap conflicts for journey X</li></ul> |
| **Journey Agent** | Journey management | Adobe Journey Optimizer (B2C and B2B Editions) | **25** | <ul><li>How many live journeys do I have?</li><li>List all journeys using the audience X.</li><li>List all journeys currently in test mode</li></ul> |
| **Product Support Agent** | Knowledge-based troubleshooting | Real-Time CDP (B2B, B2C, and B2P Editions)<br>Adobe Journey Optimizer (B2C and B2B Editions)<br>Customer Journey Analytics (B2C and B2B Editions)<br>Adobe Experience Manager | **0** | <ul><li>Why does my profile count differ on the License Usage Dashboard and the Experience Platform home page?</li><li>What are the reasons for a journey not triggering?</li><li>How does Adobe Experience Platform create real-time experiences?</li><li>How do you configure and use alerts in Adobe Experience Platform?</li><li>What is the average profile richness limit in Adobe Experience Platform Activation?</li></ul> |
| **Product Support Agent** | Support case creation and tracking | Real-Time CDP (B2B, B2C, and B2P Editions)<br>Adobe Journey Optimizer (B2C and B2B Editions)<br>Customer Journey Analytics (B2C and B2B Editions)<br>Adobe Experience Manager | **10** | <ul><li>Create a new support ticket for my failing segmentation job</li><li>What's the status of ticket E-001772068?</li></ul> |
| **Content Advisor Agent** | Content discovery | Adobe Experience Manager Cloud Services | **5** | <ul><li>Show content fragments for creating WKND offer campaign.</li><li>Find product packaging PNG images.</li><li>Show images tagged office in folder WKND.</li><li>Are there any svgs in folder WKND?</li><li>Show me all loan application forms.</li><li>I'm looking for employee onboarding forms.</li></ul> |
| **Content Advisor Agent** | Content update / optimization / forms creation | Adobe Experience Manager Cloud Services | **10** | <ul><li>Create a 2000px rendition as JPEG with 80% quality.</li><li>Create a rendition for an Instagram story.</li><li>Overlay the image with 30% discount graphics over the promotional banner, placing it 100px from the center.</li><li>Change background color of the PNG to #ff8932.</li></ul> |
| **Brand Experience Agent** | Experience production / development support | Adobe Experience Manager Cloud Services | **5** | <ul><li>Troubleshoot my failed pipeline</li><li>List my failed pipelines for Main Program.</li><li>Analyze my failed pipeline called "Dev Pipeline."</li><li>Troubleshoot pipeline execution 1234567</li></ul> |










>[!NOTE]
>
>Actual AI credit consumption may vary depending on the number of steps executed and iterations per step.

## More help on this topic

* [Agentic AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Adobe Experience Platform Agents usage-bound trial](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)