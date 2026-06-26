# Blueshift MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blueshift)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Orchestrate customer engagement via Blueshift — manage campaigns, track events, and sync customer data directly from any AI agent.

## Description
Connect your **Blueshift** account to any AI agent and orchestrate your omnichannel marketing and customer data workflows through natural conversation.

### What you can do

- **Campaign Management** — List all marketing campaigns, retrieve detailed execution reports, and monitor high-level performance.
- **Customer Data Orchestration** — Retrieve and update detailed customer profiles, including custom attributes and identifiers.
- **Real-time Event Tracking** — Track custom user interactions (purchases, clicks, views) and retrieve event histories for behavior analysis.
- **Catalog & Segment Discovery** — List all data catalogs and customer segments to ensure accurate targeting.
- **Triggered Campaigns** — Initiate API-triggered campaigns for specific users directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Blueshift User API Key and Site ID
3. Start managing your customer engagement from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Operations** — quickly check campaign statuses and customer profiles without manual dashboard searches.
- **CRM Specialists** — monitor real-time event tracking and customer attributes straight from their workflow tools.
- **Growth Engineers** — verify API integrations and campaign triggers using natural language.


## Available Tools (10)
- **list_segments**: List all customer segments
- **create_update_customer**: Create or update a customer profile
- **list_campaigns**: List all marketing campaigns
- **list_catalogs**: List all data catalogs
- **track_event**: Track a custom user event
- **get_campaign_detail**: Get detailed report for a specific campaign
- **get_campaign_performance**: Get high-level performance summary for all campaigns
- **get_catalog_items**: Retrieve items from a specific catalog
- **get_customer**: Retrieve a customer profile
- **get_event_history**: Get history of events for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blueshift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in Blueshift."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Welcome Series V2', 'Summer Re-engagement', and 'Cart Abandonment'.

---

**👤 You:**
> "Show the profile for customer john@example.com."

**🤖 AI Agent:**
> I found the profile for John Doe. Key attributes include: Member since 2023, Total spent $450, and 5 active segments including 'High Value Customers'.

---

**👤 You:**
> "Track a 'purchase' event for user customer_123."

**🤖 AI Agent:**
> Successfully tracked the 'purchase' event for customer_123. The data has been synced to Blueshift and will be reflected in their activity timeline.


## ❓ FAQ

**Q: Can I check the latest events tracked for a specific customer?**
Yes! Use the `get_event_history` tool with the customer's email or ID. Your agent will fetch the timeline of their interactions, such as purchases or email opens.

**Q: How do I see the performance summary of my current campaigns?**
Simply ask the agent to `get_campaign_performance`. It will retrieve a high-level overview of metrics across all active and past campaigns in your account.

**Q: Does the integration allow updating customer attributes?**
Yes. Use the `create_update_customer` tool to modify profile data such as first name, last name, or custom properties directly from the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blueshift](https://vinkius.com/mcp/blueshift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blueshift** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blueshift` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blueshift** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blueshift": {
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
