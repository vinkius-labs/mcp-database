# Giftpack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giftpack-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send corporate gifts at scale with AI-curated selections that match recipient preferences and company budget guidelines.

## Description
Connect your **Giftpack** account to any AI agent and take full control of your corporate gifting and employee recognition workflows through natural conversation.

### What you can do

- **Gifting Orchestration** — Send curated, personalized gifts to employees or clients globally and retrieve detailed metadata and real-time tracking programmatically
- **Campaign Management** — Create and monitor corporate gifting drives and retrieve comprehensive engagement statistics and fulfillment status
- **Catalog Intelligence** — Search through millions of high-quality gift options filtered by category and region directly through your agent
- **Recipient CRM** — Manage and retrieve detailed recipient profiles and their complete gifting history to maintain high-fidelity relationships
- **Order Monitoring** — Check order statuses and manage delivery logistics programmatically to ensure a perfect gifting experience

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Giftpack dashboard (Settings / API)
3. Start managing your corporate incentives from Claude, Cursor, or any MCP client

No more manual ordering or complex shipping tracking through fragmented emails. Your AI acts as your dedicated gifting and logistics coordinator.

### Who is this for?

- **HR Managers** — instantly automate welcome kits and work anniversary gifts using natural language queries
- **Sales Teams** — send personalized thank-you gifts to clients and monitor delivery without leaving your workspace
- **Marketing Leaders** — coordinate large-scale brand ambassador gifting campaigns and track budget utilization


## Available Tools (12)
- **create_campaign**: Requires a title and campaign details.

Start a new gifting campaign
- **trigger_gift_send**: Send a gift to a recipient
- **create_recipient**: Requires name and email.

Add a new recipient
- **get_campaign_statistics**: Get analytics for a campaign
- **get_order_fulfillment_status**: Track a gift order
- **get_product_details**: Get details for a specific gift product
- **get_recipient_details**: Get details for a specific recipient
- **list_gifting_campaigns**: List all gifting campaigns
- **list_gift_orders**: List recent gift orders
- **list_recipients**: List gift recipients
- **list_active_webhooks**: List gift event webhooks
- **search_gift_catalog**: g., category or region).

Search the Giftpack product catalog


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Giftpack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active gifting campaigns in my Giftpack account."

**🤖 AI Agent:**
> I've retrieved your active campaigns. You have 2 drives running: 'New Hire Welcome 2026' (ID: camp_123) and 'Global Client Rewards' (ID: camp_456). Would you like the engagement stats for either of these?

---

**👤 You:**
> "Send a 'Wellness Kit' to Jane Doe (ID: rec_789)."

**🤖 AI Agent:**
> Gifting triggered! I've initiated a new order for Jane Doe (ID: rec_789) with the product 'Wellness Kit' (ID: prod_001). The order ID is 'ord_101'. I'll alert you as soon as the fulfillment status changes.

---

**👤 You:**
> "Check the delivery status of order 'ord_101'."

**🤖 AI Agent:**
> Tracking order ord_101... The gift is currently 'In Transit' via FedEx and is expected to arrive at the recipient's location in London by tomorrow. Here is the tracking link: [link].


## ❓ FAQ

**Q: How do I find my Giftpack API Key?**
Log in to your Giftpack business dashboard and navigate to the **Settings** or **API** section to generate your unique key.

**Q: Can I search for gifts in a specific region?**
Yes! The `search_gift_catalog` tool allows you to include regional filters in your query to find products available for specific countries.

**Q: How do I track the delivery status of a gift?**
Use the `get_order_fulfillment_status` tool with the unique order ID to retrieve real-time shipping updates and tracking links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giftpack-alternative](https://vinkius.com/mcp/giftpack-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Giftpack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `giftpack-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Giftpack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "giftpack-alternative": {
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
