# LeadsRx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leadsrx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Analyze marketing attribution and track conversions via LeadsRx — get campaign results and touchpoint insights directly from your AI agent.

## Description
Connect your **LeadsRx** account to your AI agent and gain deep insights into your marketing performance and customer journeys through natural conversation.

### What you can do

- **Campaign Analysis** — Retrieve attribution results for specific marketing campaigns to understand ROI and performance.
- **Conversion Tracking** — List all defined conversions and programmatically add new conversion events.
- **Touchpoint & Channel Insights** — Access and list your marketing touchpoints and top-level channels to see where your customers are coming from.
- **Ecosystem Oversight** — List associated marketing agencies and advertisers managed under your profile.
- **Deep Inspection** — Fetch detailed metadata and performance metrics for specific touchpoints or conversions.

### How it works

1. Subscribe to this server
2. Enter your LeadsRx API Key
3. Start analyzing your marketing attribution from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — instantly check campaign performance and attribution metrics without opening the LeadsRx dashboard.
- **Data Analysts** — automate the retrieval of touchpoint and conversion data for deeper reporting.
- **Growth Teams** — verify the success of new marketing initiatives and track conversions in real-time.


## Available Tools (10)
- **add_conversion**: Add a new conversion event
- **get_campaign_results**: Get attribution results for a campaign
- **get_conversion_details**: Get specific conversion info
- **get_touchpoint_details**: Get specific touchpoint details
- **list_advertisers**: List connected advertisers
- **list_agencies**: List associated marketing agencies
- **list_campaigns**: List marketing campaigns
- **list_channels**: g., Social, Search, Email) defined in your account.

List marketing channels
- **list_conversions**: List all LeadsRx conversions
- **list_touchpoints**: List marketing touchpoints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LeadsRx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the attribution results for campaign 'Q1-SOCIAL-AD'."

**🤖 AI Agent:**
> I've retrieved the results for 'Q1-SOCIAL-AD'. This campaign has generated 156 conversions with an attributed credit of $4,500.00. The primary touchpoint was 'Facebook Ads'. Would you like to see the full breakdown of touchpoints?

---

**👤 You:**
> "List all our active marketing campaigns."

**🤖 AI Agent:**
> I've fetched your active campaigns. You have 8 campaigns running, including 'Google Search - Brand', 'Retargeting Promo', and 'Influencer Outreach'. Shall I retrieve the conversion details for any of these?

---

**👤 You:**
> "Show me our marketing channels and touchpoints."

**🤖 AI Agent:**
> Retrieving your marketing ecosystem... I found 5 primary channels (Search, Social, Display, Email, Referral) and a total of 24 active touchpoints. Would you like to see the performance of the 'Search' channel specifically?


## ❓ FAQ

**Q: Can I add conversions manually through the agent?**
Yes. Use the `add_conversion` tool by providing a Conversion ID and a value. This is useful for tracking offline or server-side events directly from your chat.

**Q: How do I find a specific Campaign ID?**
You can use the `list_campaigns` tool to see all active and historical campaigns along with their unique identifiers.

**Q: Does this support multi-touch attribution?**
Yes, LeadsRx is built for multi-touch attribution. This server provides the data based on the attribution models configured in your LeadsRx dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leadsrx](https://vinkius.com/mcp/leadsrx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LeadsRx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leadsrx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LeadsRx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leadsrx": {
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
