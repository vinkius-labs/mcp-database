# Bloomreach MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bloomreach)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage your marketing automation via Bloomreach — list catalogs, campaigns, and customer segments directly from any AI agent.

## Description
Connect your **Bloomreach Engagement** account to any AI agent and orchestrate your marketing automation and data workflows through natural conversation.

### What you can do

- **Catalog Oversight** — List and retrieve items from your data catalogs to ensure product and metadata accuracy.
- **Campaign Management** — Query and monitor marketing campaigns to track outreach and performance.
- **Customer Segmentation** — Access and list customer segments and segmentations for targeted marketing analysis.
- **Event Tracking Discovery** — List all tracked event types to understand your data collection footprint.
- **Attribute & Property Auditing** — Retrieve configured customer attributes and catalog properties.
- **Webhook Monitoring** — List configured webhooks to verify real-time data integrations.

### How it works

1. Subscribe to this server
2. Enter your Project Token, API ID, API Secret, and Base URL
3. Start managing your marketing ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly check catalog data and campaign statuses without manual exports.
- **CRM Specialists** — monitor customer segments and event tracking straight from their workflow tools.
- **Data Analysts** — retrieve attribute and property definitions using natural language.


## Available Tools
- **get_catalog_items**: Retrieve items from a specific data catalog
- **get_customer_properties**: Export properties for a specific registered customer
- **list_segmentations**: List all customer segmentations
- **list_attributes**: List all customer attributes
- **list_campaigns**: List all marketing campaigns
- **list_catalogs**: List all Bloomreach data catalogs
- **list_event_types**: List all tracked event types
- **list_properties**: List all catalog properties
- **list_segments**: List all customer segments
- **list_webhooks**: List configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bloomreach** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in Bloomreach."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Summer Sale Newsletter', 'Re-engagement Q2', and 'Abandoned Cart Recovery'.

---

**👤 You:**
> "Show me the items in the 'Top Products' catalog."

**🤖 AI Agent:**
> Retrieving items for 'Top Products'... I found 5 items, including 'Leather Backpack' (ID: prod_1) and 'Wireless Headphones' (ID: prod_2). Would you like the full metadata for any item?

---

**👤 You:**
> "List all customer segments."

**🤖 AI Agent:**
> I've retrieved your segments. You have groups like 'High Spenders', 'Recent Visitors', and 'Loyalty Members'. Which one would you like to explore?


## ❓ FAQ

**Q: Can I check the items in a specific data catalog?**
Yes! Use the `get_catalog_items` tool with the Catalog ID. Your agent will fetch the items and their metadata directly from your Bloomreach instance.

**Q: How do I see all the customer segments I have created?**
Simply ask the agent to `list_segments` or `list_segmentations`. It will retrieve the definitions and names of the customer groups you've configured in the Engagement platform.

**Q: Does the integration allow exporting customer properties?**
Yes. Use the `get_customer_properties` tool with a registered Customer ID. The agent will retrieve core properties like name and email based on your project configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bloomreach](https://vinkius.com/mcp/bloomreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bloomreach** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `bloomreach` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bloomreach** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bloomreach": {
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
