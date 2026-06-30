# Ometria Intelligence MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ometria-intelligence)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Analyze customer data and retail marketing via Ometria — track contacts, orders, and segments directly from your AI agent.

## Description
Connect your **Ometria** account to your AI agent and gain deep visibility into your customer life cycle and retail marketing performance through natural conversation.

### What you can do

- **Customer Oversight** — List and inspect customer profiles, including their attributes, segments, and lifetime value.
- **Order Tracking** — Access recent customer orders and transactions, including full metadata and status updates.
- **Product Intelligence** — View your entire product catalog and check specific item metadata and stock statuses.
- **Segment Analysis** — List audience segments defined in Ometria and retrieve member counts for targeting.
- **Campaign Performance** — Monitor email and automation campaigns and fetch real-time engagement statistics.
- **Transactional Monitoring** — View recent customer interactions and goal completions across your marketing funnel.
- **Deep Inspection** — Fetch complete metadata for specific contacts, orders, or campaigns using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Ometria API Key (X-Ometria-Auth)
3. Start exploring customer intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **CRM Managers** — quickly check customer segment sizes or individual profile details without opening the portal.
- **E-commerce Operations** — monitor recent order statuses and product catalog updates in real-time.
- **Marketing Analysts** — automate the retrieval of campaign performance stats and audience metrics.


## Available Tools (10)
- **get_order_details**: Get specific order details
- **get_product_details**: Get specific product info
- **get_segment_details**: Get specific segment info
- **list_marketing_campaigns**: List marketing campaigns
- **list_contacts**: List customer contacts
- **list_orders**: List customer orders
- **list_catalog_products**: List product catalog
- **list_customer_segments**: List customer segments
- **get_campaign_stats**: Get campaign performance stats
- **get_contact_details**: Get specific contact info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ometria Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns."

**🤖 AI Agent:**
> Retrieving campaigns... I found 12 active campaigns including 'Spring Sale 2024', 'Welcome Automation', and 'VIP Loyalty Program'. Would you like the engagement stats for the Spring Sale?

---

**👤 You:**
> "What is the status of order ID 'ord_98765'?"

**🤖 AI Agent:**
> Inspecting order ord_98765... The order is currently 'Shipped' and was placed yesterday. It contains 3 items totaling $145.00. Shall I list the contact details for the customer who placed this order?

---

**👤 You:**
> "Show me the details for the 'High LTV' segment."

**🤖 AI Agent:**
> Fetching segment details... The 'High LTV' segment currently contains 1,250 members. This audience consists of customers who have placed at least 5 orders in the last 12 months. Would you like to see the recent order history for this group?


## ❓ FAQ

**Q: How do I get an Ometria API Key?**
You can generate an API key in the Ometria settings dashboard under the API tab. This key should be used for the `X-Ometria-Auth` header.

**Q: Can I see customer lifetime value (LTV)?**
Yes! Use the `get_contact_details` tool with a specific contact ID to retrieve their full profile, which includes segment associations and calculated lifetime metrics.

**Q: Does this support real-time campaign stats?**
Yes, the `get_campaign_stats` tool retrieves current engagement metrics directly from Ometria for any specific campaign ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ometria-intelligence](https://vinkius.com/mcp/ometria-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ometria Intelligence** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ometria-intelligence` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ometria Intelligence** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ometria-intelligence": {
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
