# CleverTap MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clevertap)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage customer engagement and analytics via CleverTap — track campaigns, monitor user segments, and audit event data directly from any AI agent.

## Description
Connect your **CleverTap** account to any AI agent and take full control of your customer engagement and retention strategies through natural conversation. Streamline how you monitor campaigns and analyze user behavior natively.

### What you can do

- **Campaign Oversight** — List and retrieve details for all scheduled and running campaigns natively
- **Analytics Intelligence** — Access detailed performance reports including clicks, conversions, and delivery flawlessly
- **Segment Logistics** — Monitor all defined user segments to understand your audience distribution securely
- **Event Tracking** — List custom event schemas and user properties to audit data ingestion flawlessly
- **Real-time Visibility** — Access real-time usage statistics and active user counts flawlessly
- **User Deep-Dives** — Retrieve detailed profile information for specific user identities directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CleverTap Account ID, API Passcode, and Region
3. Start managing your engagement strategy from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Marketers** — monitor campaign ROI and conversion rates using natural language
- **Retention Leads** — review user segments and engagement trends without opening the dashboard
- **Product Managers** — quickly look up event schemas and real-time usage stats straight from their chat interface
- **Marketing Ops** — verify data ingestion and monitor campaign delivery health


## Available Tools (8)
- **get_campaign_performance_report**: Retrieve detailed performance metrics for a specific campaign
- **get_user_profile_details**: Get detailed information for a specific user identity
- **get_real_time_usage_stats**: Retrieve real-time user counts and event statistics
- **list_clevertap_apps**: List all applications registered in the account
- **list_event_schemas**: List all custom events and their schemas
- **list_clevertap_campaigns**: List all campaigns scheduled within a date range
- **list_clevertap_segments**: List all defined user segments
- **list_user_profile_properties**: List all user profile properties and attributes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CleverTap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my CleverTap campaigns from last month."

**🤖 AI Agent:**
> Retrieving campaigns from last month... I found 5 items: 'Summer Sale Push' (Completed), 'Welcome Email Series' (Running), and 3 others. Would you like the performance report for any of these?

---

**👤 You:**
> "What is the performance report for campaign ID 1457432732?"

**🤖 AI Agent:**
> Checking performance for campaign 1457432732... This campaign sent 50,000 messages, had 4,500 clicks (9% CTR), and resulted in 1,200 conversions (2.4% conversion rate).

---

**👤 You:**
> "Show me the custom event schemas in my account."

**🤖 AI Agent:**
> Retrieving event schemas... You have 12 custom events defined, including 'Product Viewed', 'Add to Cart', 'Charged', and 'Search Executed'. I can provide the attributes for any of these.


## ❓ FAQ

**Q: Can I see the conversion rate for a specific campaign?**
Yes! Use the `get_campaign_performance_report` tool with the campaign ID. The agent will return detailed metrics including total conversions and the calculated conversion percentage from CleverTap.

**Q: How do I check the definition of a specific user segment?**
Use the `list_clevertap_segments` tool. Your agent will fetch all segments configured in your account, allowing you to review their names and core identifiers.

**Q: Where do I find my CleverTap Account ID and API Passcode?**
Log in to your CleverTap dashboard, navigate to **Settings**, and select **Dashboard Settings**. You will find your Project ID (Account ID) and API Passcode there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clevertap](https://vinkius.com/mcp/clevertap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CleverTap** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clevertap` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CleverTap** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clevertap": {
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
