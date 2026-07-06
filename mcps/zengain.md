# Zengain MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zengain)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Identify high-intent website visitors by company and reach out to warm leads before they fill out a form or contact you.

## Description
Connect your **Zengain** (Nalpeiron Growth Platform) account to any AI agent and simplify your customer success and usage analytics workflows through natural conversation.

### What you can do

- **Product Lifecycle** — List all registered products and retrieve detailed configuration metadata
- **User Engagement** — Query product users, inspect their profiles, and calculate real-time health scores
- **Usage Analytics** — Get high-level analytics summaries and track custom events to monitor feature adoption
- **KPM Tracking** — Monitor Key Product Milestones to identify successful onboarding and churn risks
- **System Monitoring** — List configured webhooks to understand your integration data flow

### How it works

1. Subscribe to this server
2. Enter your Zengain Tenant ID and API Key
3. Start managing your customer success resources from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **list_kpms**: List Key Product Milestones
- **list_products**: List Zengain products
- **list_users**: List product users
- **list_webhooks**: List configured webhooks
- **track_event**: Track a custom event
- **get_health_score**: Get customer health score
- **get_product**: Get details for a specific product
- **get_analytics_summary**: Get analytics summary
- **get_user_details**: Get details for a specific user
- **list_events**: List tracking events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zengain** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Zengain account."

**🤖 AI Agent:**
> I've found 3 products: 'Desktop App v2', 'Cloud SaaS Portal', and 'Mobile Lite'. Which one should I analyze?

---

**👤 You:**
> "What is the health score for user 'customer_456'?"

**🤖 AI Agent:**
> User 'customer_456' has a health score of 82/100 (Good). Their engagement has increased by 15% over the last 30 days.

---

**👤 You:**
> "Show me a summary of usage analytics for this month."

**🤖 AI Agent:**
> Across all products, you have 1,200 Daily Active Users (DAU) and 5,500 Monthly Active Users (MAU). Feature adoption for 'Real-time Sync' is at an all-time high.


## ❓ FAQ

**Q: Can I calculate a customer's health score using my AI agent?**
Yes! Use the `get_health_score` tool by providing the User ID. The agent will retrieve the real-time engagement score from Zengain.

**Q: How do I see high-level usage summary for a specific product?**
Use the `get_analytics_summary` tool. You can optionally provide a Product ID to filter the metrics for that specific offering.

**Q: Is it possible to track a new custom event through this integration?**
Yes, use the `track_event` action. Provide the User ID and the Event Name to record engagement data programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zengain](https://vinkius.com/mcp/zengain)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zengain** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zengain` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zengain** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zengain": {
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
