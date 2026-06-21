# Offerslook MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/offerslook)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage performance marketing via Offerslook — track offers, advertisers, and affiliates directly from your AI agent.

## Description
Connect your **Offerslook** network account to your AI agent and streamline your performance marketing operations and partner management through natural conversation.

### What you can do

- **Offer Management** — List all active and paused marketing offers and retrieve detailed payout and tracking configuration.
- **Partner Oversight** — Access profiles and performance settings for all advertisers and affiliates in your network.
- **Campaign Tracking** — View active marketing campaigns and monitor recent conversion history in real-time.
- **Performance Reporting** — Generate aggregated reports for specific date ranges to track clicks, conversions, and revenue.
- **Category Discovery** — Browse the organizational categories used to group and manage your offers.
- **Deep Inspection** — Fetch complete metadata for specific offers, partners, or campaigns using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Offerslook Network ID and API Key
3. Start managing your marketing network from Claude, Cursor, or any MCP client

### Who is this for?

- **Affiliate Managers** — quickly check offer statuses or partner details without opening the dashboard.
- **Network Administrators** — monitor campaign distribution and conversion trends directly from your workspace.
- **Marketing Analysts** — automate the retrieval of performance reports and partner data for analysis.


## Available Tools
- **get_advertiser_details**: Get specific advertiser details
- **get_affiliate_details**: Get specific affiliate details
- **get_offer_details**: Get specific offer info
- **get_performance_report**: Generate performance report
- **list_advertisers**: List all advertisers
- **list_affiliates**: List all affiliates/publishers
- **list_active_campaigns**: List marketing campaigns
- **list_offer_categories**: List offer categories
- **list_recent_conversions**: List recent conversions
- **list_offers**: List all marketing offers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Offerslook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active offers in my network."

**🤖 AI Agent:**
> Retrieving offers... I found 15 active offers including 'E-commerce Summer Sale', 'VPN Pro Trial', and 'Flash Deal'. Would you like the payout details for the Summer Sale?

---

**👤 You:**
> "What is the status of advertiser ID 'adv_98765'?"

**🤖 AI Agent:**
> Inspecting advertiser adv_98765... The profile belongs to 'Global Brands Inc.'. It is currently 'Active' and has 3 running campaigns. Shall I list their recent conversion metrics?

---

**👤 You:**
> "Show me the performance report for the first week of March."

**🤖 AI Agent:**
> Generating performance report... For the week of March 1st to March 7th, your network generated 45,000 clicks and 1,250 conversions, resulting in $8,400 in revenue. Would you like to see which affiliate performed best during this period?


## ❓ FAQ

**Q: Where do I find my Offerslook API Key?**
Log in to your Offerslook network dashboard and navigate to the API settings section to find your Network ID and API Key.

**Q: Can I see conversions in real-time?**
Yes! Use the `list_recent_conversions` tool to retrieve a list of the latest successful goal completions in your network.

**Q: How do I generate a performance report?**
The `get_performance_report` tool allows you to specify a start and end date to retrieve aggregated metrics for your network.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/offerslook](https://vinkius.com/mcp/offerslook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Offerslook** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `offerslook` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Offerslook** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "offerslook": {
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
