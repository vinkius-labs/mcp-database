# MerchantSpring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/merchantspring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Cross-marketplace reporting via MerchantSpring — track sales, orders, and products from multiple stores.

## Description
Connect your **MerchantSpring** account to any AI agent and take full control of your e-commerce performance and cross-marketplace data through natural conversation.

### What you can do

- **Unified Reporting** — Retrieve aggregated sales summaries and performance metrics across all your connected marketplaces
- **Store Orchestration** — List all connected store accounts and fetch detailed metadata and health statuses
- **Order Management** — List and inspect order histories for specific stores including Amazon, eBay, and more
- **Catalog Visibility** — Access product listings and detailed inventory reports for your multi-channel operations
- **Alert Monitoring** — Track active marketplace notifications and store alerts directly from your agent

### How it works

1. Subscribe to this server
2. Enter your MerchantSpring API Key
3. Start managing your e-commerce intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_store_health**: Get store health status
- **get_inventory_report**: Get inventory status report
- **get_sales_summary**: Get aggregated sales summary
- **get_store_details**: Get details for a specific store
- **list_merchant_alerts**: List all marketplace alerts
- **list_marketplaces**: g. Amazon, eBay).

List all supported marketplaces
- **list_store_orders**: List orders for a specific store
- **list_store_products**: List products for a specific store
- **list_store_promotions**: List active store promotions
- **list_stores**: List all connected stores


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MerchantSpring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a sales summary for all my stores this month."

**🤖 AI Agent:**
> Retrieving summary... You have total sales of $45,000 across 5 stores, with Amazon being your top performer.

---

**👤 You:**
> "List all products for store ID 'S_98765'."

**🤖 AI Agent:**
> Querying products... Store 'S_98765' has 150 active listings, including 'Blue Widget' and 'Red Gadget'.

---

**👤 You:**
> "Check health status for my connected stores."

**🤖 AI Agent:**
> Checking health... 4 stores are healthy, but your eBay AU store has a sync alert regarding inventory levels.


## ❓ FAQ

**Q: How do I find my MerchantSpring API Key?**
Log in to MerchantSpring, navigate to your Profile (top right), and look for the API section to generate your key.

**Q: What marketplaces are supported?**
MerchantSpring supports over 120 marketplaces including Amazon, eBay, Walmart, Shopify, and many regional platforms.

**Q: Is my marketplace data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/merchantspring](https://vinkius.com/mcp/merchantspring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MerchantSpring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `merchantspring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MerchantSpring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "merchantspring": {
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
