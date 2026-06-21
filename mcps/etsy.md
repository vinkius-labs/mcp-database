# Etsy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/etsy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Etsy shop — audit listings, orders, and reviews via AI.

## Description
Empower your AI agent to orchestrate your entire handmade and vintage marketplace ecosystem with **Etsy**, the global destination for unique and creative goods. By connecting Etsy to your agent, you transform complex shop management into a natural conversation. Your agent can instantly list your active inventory, audit recent customer reviews, and retrieve order receipts without you ever touching a dashboard. Whether you are an independent artisan or a high-volume seller, your agent acts as a real-time shop operator, ensuring your listings are always optimized and your customers are well-served.

### What you can do

- **Inventory Auditing** — List all listings in your shop and retrieve detailed metadata, including pricing, state, and URLs.
- **Order Management** — Browse shop receipts to maintain a clear view of your recent sales and fulfillment status.
- **Review Oversight** — List all customer reviews for your shop to stay on top of your brand reputation and feedback.
- **Listing Governance** — Update listing titles and descriptions through natural language to keep your catalog current.
- **Market Intelligence** — Search for active listings across the Etsy platform to find inspiration or monitor competition.

### How it works

1. Subscribe to this server
2. Enter your Etsy API Key and Access Token
3. Start managing your handmade business through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Shop Owners** — monitor inventory levels and order statuses straight from your creative workflow.
- **Marketing Leads** — verify if new listings have been correctly published and described for maximum reach.
- **Support Teams** — perform rapid review audits and check customer order details without manual dashboard logins.
- **Operations Managers** — automate shop querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **get_listing**: Get details for a specific listing
- **get_me**: Get authenticated user and application info from Etsy
- **get_receipt**: Get details for a specific receipt
- **get_shop**: Get details for a specific Etsy shop
- **list_shop_listings**: List listings for a specific shop
- **list_shop_receipts**: List receipts (orders) for a shop
- **list_shop_reviews**: List reviews for a shop
- **list_shop_sections**: List sections for a shop
- **search_active_listings**: Search for active listings on Etsy
- **update_listing**: Update an Etsy listing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Etsy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active listings in shop ID xxxx."

**🤖 AI Agent:**
> I've retrieved your active inventory. You have 12 listings, including 'Handmade Vase' and 'Vintage Watch'. Would you like the pricing for any of them?

---

**👤 You:**
> "Show me the last 5 reviews for my Etsy shop."

**🤖 AI Agent:**
> I've found the last 5 reviews. Most customers are giving 5 stars, praising the 'fast shipping'. One customer mentioned 'beautiful packaging'. Would you like to see the full comments?

---

**👤 You:**
> "Search for active listings with keyword 'linen dress'."

**🤖 AI Agent:**
> I've found several matching listings for 'linen dress'. Top results include 'Handmade Linen Summer Dress' and 'Boho Linen Tunic'. Would you like the direct links to view them?


## ❓ FAQ

**Q: How do I find my Etsy API Key and Access Token?**
Register an App in the [**Etsy Developer Console**](https://www.etsy.com/developers/register) to get your Keystring, then perform the OAuth flow to generate an Access Token. Copy and paste them below.

**Q: Can the agent list my recent sales receipts?**
Yes. Use the `list_shop_receipts` tool providing your Shop ID. Your agent will retrieve the most recent transactions, including payment and shipping statuses.

**Q: Is it possible to update an Etsy listing via the agent?**
Yes. The `update_listing` tool allows your agent to modify existing listing titles and descriptions instantly by providing the specific Listing ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/etsy](https://vinkius.com/mcp/etsy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Etsy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `etsy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Etsy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "etsy": {
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
