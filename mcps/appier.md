# Appier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Empower your AI agents to manage Appier campaigns, analyze predictive audiences, and fetch real-time conversion metrics directly from chat.

## Description
Connect your **Appier** environment to any AI agent and bring the power of AI-driven marketing campaigns directly into your chat interface. Skip the complex dashboards and interact with your predictive segments, marketing performance, and conversion tracking using natural language.

### What you can do

- **Campaign Management** — List all active CrossX or AIQUA campaigns and drill down into specific campaign configurations instantly
- **Audience & Segments** — Retrieve AI-generated audiences, view segment sizes, and understand criteria predicting user behavior
- **Predictive Models** — List actively running ML predictions like Churn and Purchase probability models
- **Conversion Tracking** — View historical tracked conversion events like signups or purchases
- **Performance Analytics** — Fetch full analytics (CTR, CPC, ROAS, and Conversions) for any given campaign

### How it works

1. Subscribe to this server
2. Enter your Appier API Key and API URL
3. Start fetching ROAS reports or audience sizes directly from Claude, Cursor, or any MCP-compatible platform

### Who is this for?

- **Growth Marketers** — fetch ROAS and CPC metrics across campaigns continuously without leaving your strategy documents
- **Data Analysts** — parse active ML predictive models and segmentation rules directly alongside your code
- **Marketing Leadership** — prompt agents to summarize campaign statuses and overall conversions before a meeting
- **E-commerce Teams** — track recent high-value conversions dynamically based on predictive segments


## Available Tools (8)
- **list_campaigns**: List all AI marketing campaigns in Appier
- **get_campaign**: Get specific marketing campaign details
- **list_audiences**: List all target audiences
- **get_audience**: Get details for a specific audience
- **list_segments**: List configured user segments
- **list_predictions**: List available AI prediction models
- **list_conversions**: List tracked conversion events
- **get_campaign_analytics**: Get analytics and performance metrics for a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns we have on Appier."

**🤖 AI Agent:**
> You currently have 4 active campaigns. They include 'Q3 Retargeting' (ID: cmp_q3rtg), 'High LTV Predict' (ID: cmp_ltv), and 'Abandoned Cart Rescue' (ID: cmp_abrt). Would you like to check the analytics for the High LTV campaign?

---

**👤 You:**
> "What is our current ROAS and CPC for campaign cmp_q3rtg?"

**🤖 AI Agent:**
> Here are the recent analytics for Q3 Retargeting (cmp_q3rtg): The overall Return on Ad Spend (ROAS) is at 310%. Your Cost Per Click (CPC) averages $1.15. You have a total of 1450 conversions traced so far. Should we cross-reference this with the list of active audiences?

---

**👤 You:**
> "What predictive models do we have running right now?"

**🤖 AI Agent:**
> You have 2 predictive models configured. The 'Churn Risk Model' predicting users likely to drop in 7 days, and the 'Purchase Propensity Engine' for identifying high-value carts. I can pull the specific data segments grouped under the Churn Model if you need to take action.


## ❓ FAQ

**Q: Can my AI agent create new predictive models in Appier?**
No. The MCP server is designed natively for reading data, fetching performance stats, analyzing segments, and understanding configurations. Creating complex models still requires the Appier Enterprise Console to ensure ML model safety.

**Q: How fast can I generate a campaign ROI report before a meeting?**
In a few seconds. Tell your agent 'Fetch analytics for my top 3 active campaigns' and the AI will invoke the analytics endpoint, process the CPC, CTR, and ROAS data, and output a clean executive summary in whatever format you ask.

**Q: Can the agent tell me how big a specific prediction segment is?**
Yes. If an audience ID or segment ID is known, the agent uses the 'get_audience' tool to fetch size estimations, AI criteria, and generation metrics—informing you immediately if your targeted audience size is large enough to launch.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appier](https://vinkius.com/mcp/appier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appier": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
