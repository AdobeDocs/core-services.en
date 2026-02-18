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

| Agent | Job | Supported applications | Estimated AI credits | Sample prompts |
| ------ |-----|------------------------|----------------------|----------------|
| Audience Agent | Audience / account ideation | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 50 | <ul><li>_Show me fields for affluent buyers_</li><li>_Find all fields related to customer preferences_</li></ul> |
| Audience Agent | Knowledge-based audience / account creation | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 150 | <ul><li>_Create an audience made up of people who live in California_</li><li>_Generate an audience of VIP members who spent over $1000 this quarter_</li><li>_Build an audience of users who bought clothing items but haven't made a purchase in the last 60 days_</li></ul> |
| Audience Agent | Audience / account management | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>_Do I have any duplicate audiences?_</li><li>_Show me my 5 largest audiences._</li><li>_Show me audiences that are not activated to any destination_</li><li>_List all audiences used in live journeys_</li></ul> |
| Audience Agent | Audience / account analysis | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2C Edition)</li></ul> | 25 | <ul><li>_Which audiences have increased in size by more than 20% in the last week?_</li><li>_How much has audience "Loyal Platinum" changed compared to the value 30 days ago?_</li><li>_What is my fastest growing audience?_</li></ul> |
| Audience Agent | Buying group ideation | <ul><li>Adobe Journey Optimizer (B2B Edition)</li></ul> | 25 | <ul><li>_Which accounts are showing intent for these products?_</li><li>_Show me the top persons by product intent for XYZ._</li><li>_Which buying groups have more than 5 members?_</li></ul> |
| Data Insights Agent | Data analysis and visualization | <ul><li>Customer Journey Analytics (B2C and B2B Editions)</li></ul> | 25 | <ul><li>_Trend orders in July_</li><li>_Show revenue by region._</li><li>_Show orders by gender, from March to June._</li><li>_What were my top 10 SKUs by profit in June_</li><li>_Proportion of purchases by month of year_</li><li>_Share of revenue by product category_</li></ul> |
| Journey Agent | Journey ideation | <ul><li>Adobe Journey Optimizer (B2B Edition)</li></ul> | 25 | <ul><li>_Create a journey for whitespace accounts with intent for my solution, focusing on people engaged with content on the website_</li></ul> |
| Journey Agent | Journey creation | <ul><li>Adobe Journey Optimizer (B2B and B2C Editions)</li></ul> | 30 | <ul><li>_Generate a journey to send a reminder to users who have not completed their first purchase in the last 7 days_</li><li>_When users complete their first purchase, send an SMS confirmation and follow-up benefits explanation via email after 3 days_</li></ul> |
| Journey Agent | Journey analysis | <ul><li>Adobe Journey Optimizer (B2B and B2C Editions)</li></ul> | 50 | <ul><li>_I want to analyze the fallout by node for journey Fourth of July Campaign._</li><li>_Are there any scheduling conflicts for journey X_</li><li>_Show me audience overlap conflicts for journey X_</li></ul> |
| Journey Agent | Journey management | <ul><li>Adobe Journey Optimizer (B2B and B2C Editions)</li></ul> | 25 | <ul><li>_How many live journeys do I have?_</li><li>_List all journeys using the audience X._</li><li>_List all journeys currently in test mode_</li></ul> |
| Product Support Agent | Knowledge-based troubleshooting | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li><li>Adobe Journey Optimizer (B2C and B2B Editions)</li><li>Customer Journey Analytics (B2C and B2B Editions)</li></ul> | 0 | <ul><li>_Why does my profile count differ on the License Usage Dashboard and the Experience Platform home page?_</li><li>_What are the reasons for a journey not triggering?_</li><li>_How does Adobe Experience Platform create real-time experiences?_</li><li>_How do you configure and use alerts in Adobe Experience Platform?_</li><li>_What is the average profile richness limit in Adobe Experience Platform Activation?_</li></ul> |
| Product Support Agent | Support case creation and tracking | <ul><li>Real-Time CDP (B2B, B2C, and B2P Editions)</li>Adobe Journey Optimizer (B2C and B2B Editions)<li>Customer Journey Analytics (B2C and B2B Editions)</li><li>Adobe Experience Manager</li></ul> | 10 | <ul><li>_Create a new support ticket for my failing segmentation job_</li><li>_What's the status of ticket E-001772068?_</li></ul> |
| Content Advisor Agent | Content discovery | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 | <ul><li>_Show content fragments for creating WKND offer campaign._</li><li>_Find product packaging PNG images._</li><li>_Show images tagged office in folder WKND._</li><li>_Are there any svgs in folder WKND?_</li><li>_Show me all loan application forms._</li><li>_I'm looking for employee onboarding forms._</li></ul> |
| Content Advisor Agent |  <ul><li>Content update</li><li>Content optimization</li><li>Forms creation</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 10 | <ul><li>_Create a 2000px rendition as JPEG with 80% quality._</li><li>_Create a rendition for an Instagram story._</li><li>_Overlay the image with 30% discount graphics over the promotional banner, placing it 100px from the center._</li><li>_Change background color of the PNG to #ff8932._</li></ul> |
| Brand Experience Agent | <ul><li>Experience Support</li><li>Deployment support</li></ul> | <ul><li>Adobe Experience Manager Cloud Services</li></ul> | 5 | <ul><li>_Troubleshoot my failed pipeline_</li><li>_List my failed pipelines for Main Program._</li><li>_Analyze my failed pipeline called "Dev Pipeline."_</li><li>_Troubleshoot pipeline execution 1234567_</li></ul> |
| Brand Experience Agent | Site modernization | Adobe Experience Manager Cloud Services | 100 | <ul><li>_Migrate the page `https://wknd-trendsetters.site`_</li></ul> |

>[!NOTE]
>
>Actual AI credit consumption may vary depending on the number of steps executed and iterations per step.

## More help on this topic

* [Agentic AI in Experience Cloud](/help/interface/features/agentic-ai.md)
* [Adobe Experience Platform Agents usage-bound trial](https://experienceleague.adobe.com/en/docs/experience-cloud-ai/experience-cloud-ai/agents/trial)