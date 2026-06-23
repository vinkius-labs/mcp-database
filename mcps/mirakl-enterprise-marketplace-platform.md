# Mirakl (Enterprise Marketplace Platform) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mirakl-enterprise-marketplace-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage your enterprise marketplace via Mirakl — list global offers, track multi-vendor orders, and audit seller shops.

## Description
Connect your **Mirakl** instance to any AI agent and take full control of your enterprise marketplace operations, seller network, and global offer management through natural conversation.

### What you can do

- **Offer Orchestration** — List and retrieve detailed marketplace offers from multiple sellers, including inventory availability and specific pricing constraints directly from your agent
- **Order Monitoring** — Track multi-vendor checkout transactions and retrieve full line-item details, payment statuses, and fulfillment histories securely
- **Seller Management** — Enumerate third-party shops (sellers) active on your platform and retrieve detailed compliance profiles and operational configurations natively
- **Catalog & Category Audit** — Explore the broad platform product catalog and navigate hierarchical category trees to understand your marketplace's structural taxonomy
- **Financial Visibility** — List and audit structural accounting invoices and settlements triggered against seller shops to manage your marketplace's financial boundaries
- **Communication Stream** — Retrieve threaded messages between buyers, sellers, and operators to monitor support logs and platform interactions efficiently
- **Metadata Inspection** — Deep-dive into specific Offer or Order IDs to retrieve precise JSON representations and chronological transaction insights instantly

### How it works

1. Subscribe to this server
2. Enter your Mirakl Environment URL and API Key
3. Start managing your marketplace platform from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketplace Operators** — monitor multi-vendor order flows and seller performance through natural conversation without manual portal navigation
- **E-commerce Leads** — audit global offer distributions and category taxonomies directly from your workspace to optimize product discovery
- **Finance & Compliance Teams** — track marketplace invoices and seller compliance profiles efficiently to maintain high platform standards


## Available Tools (10)
- **list_offers**: Represents the exact live inventory binding a specific product to a specific explicit price from a Shop.

List global Marketplace offers created by multiple sellers
- **get_offer**: Get an explicit Mirakl offer entity mapping seller limits
- **list_orders**: List Mirakl marketplace multi-vendor checkout orders
- **get_order**: Get deep details tracing a specific Marketplace Order transaction
- **list_shops**: List third-party Seller accounts (Shops) operating
- **get_shop**: Get deep configurations tracking an explicit Mirakl Seller Shop
- **list_products**: List broad Platform Product Catalog nodes
- **list_categories**: g. Electronics -> Computers).

List static structural Mirakl marketplace Category Trees
- **list_messages**: List internal Marketplace communication messages
- **list_invoices**: List explicit Mirakl structural accounting invoices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mirakl (Enterprise Marketplace Platform)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active seller shops in my Mirakl marketplace"

**🤖 AI Agent:**
> I've retrieved your list of active shops. Highlights include 'Tech World' (ID: shop-123), 'Home & Garden Pro' (ID: shop-456), and 'Direct Sport' (ID: shop-789). Would you like to see the compliance status or offer count for any of these?

---

**👤 You:**
> "Show me the last 5 invoices generated for seller shops"

**🤖 AI Agent:**
> Retrieving latest invoices… I've identified 5 recent settlements. Highlights: Invoice #INV-1001 (€1,250 for Shop A), Invoice #INV-1002 (€850 for Shop B), and Invoice #INV-1003 (€45.50). Would you like to see the settlement details for the largest invoice?

---

**👤 You:**
> "Search for messages related to order ID 'order-987'"

**🤖 AI Agent:**
> Searching communication history… I've found a thread for order 'order-987' between the buyer and the seller. The customer is asking about the delivery timeframe. Would you like me to retrieve the full message content or draft a reply as the operator?


## ❓ FAQ

**Q: Can I see the price and stock for a specific seller offer through my agent?**
Yes. Use the `get_offer` tool with a specific Mirakl Offer ID. Your agent will retrieve the live inventory status and pricing mappings for that seller's listing, helping you audit availability across your marketplace instantly.

**Q: How do I check the compliance status of a third-party shop on my platform?**
The `get_shop` tool retrieves the complete operational configuration for a Shop ID. Your agent will expose the compliance constraints, seller profiles, and active flags, ensuring you can audit merchant health directly from your conversation.

**Q: Can my agent list all multi-vendor orders placed in a specific period?**
Absolutely. Use the `list_orders` tool to retrieve recent marketplace transactions. Your agent will report the order IDs, payment statuses, and line-item details, helping you monitor high-level multi-vendor checkout activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mirakl-enterprise-marketplace-platform](https://vinkius.com/mcp/mirakl-enterprise-marketplace-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mirakl (Enterprise Marketplace Platform)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mirakl-enterprise-marketplace-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mirakl (Enterprise Marketplace Platform)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mirakl-enterprise-marketplace-platform": {
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
