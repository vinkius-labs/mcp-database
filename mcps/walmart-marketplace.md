# Walmart Marketplace MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/walmart-marketplace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Walmart Marketplace catalog, inventory, and dynamic pricing natively.

## Description
### What you can do

Gain complete control over your Walmart 3P Seller operations, automating catalog and inventory management through secure APIs:

- **Manage Pricing:** Execute dynamic pricing updates, adjust base costs, and configure promotional rules.
- **Sync Inventory levels:** Automate physical stock allocation across your fulfillment centers in real time.
- **Control Catalog Items:** Publish, update, or retire SKUs efficiently directly from your workspace.

### How it works

1. **Configure OAuth:** Use your Walmart Developer Portal `CLIENT_ID` and `CLIENT_SECRET` to establish a secure connection.
2. **Set Environment:** Choose between Sandbox and Production.
3. **Execute:** Utilize the built-in capabilities to handle catalog data seamlessly.

### Who is this for?

Specifically built for **3P Sellers**, **E-Commerce Operators**, and **Catalog Integrators**.


## Available Tools (8)
- **wm_bulk_price_update**: Trigger structural feed array proxies safely uploading bulk payload tracking parameters matrices seamlessly
- **wm_get_taxonomy**: Poll safely dynamic category classification structures allocating explicitly Walmart structural node trees correctly
- **wm_get_item_status**: Analyze explicit proxy validations parsing lifecycle, buy-box limits, and errors over specific SKU constraints
- **wm_list_items**: Extract actively published 3P seller catalog explicit arrays tracing cleanly Walmart hosted structures
- **wm_retire_item**: Cleanly explicitly extract bounds unpublishing the active array securely masking from public constraints
- **wm_set_price**: Execute explicitly pricing proxy limits mapping the retail structured limits dynamically bounding safely
- **wm_setup_promotions**: Execute explicitly markdown and clearance logical arrays explicitly resolving structured payloads safely
- **wm_update_inventory**: Allocate physical logistic stock actively resolving unit values evaluating gracefully proxy limits natively


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Walmart Marketplace** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update the inventory of SKU 8291 to 50 items on fulfillment center 1000."

**🤖 AI Agent:**
> Successfully updated the inventory quantity using `wm_update_inventory`.

---

**👤 You:**
> "Find the current offer price and publish status of SKU 'LAPTOP-01'."

**🤖 AI Agent:**
> SKU 'LAPTOP-01' is 'PUBLISHED' with a current active offer price of $499.00 on the marketplace.

---

**👤 You:**
> "Increase the base price of all ASICS sneakers by 5% effectively immediately."

**🤖 AI Agent:**
> Bulk price adjustment initiated. 34 ASICS SKUs have been updated with a 5% markup submitted successfully.


## ❓ FAQ

**Q: Does this MCP server process fulfillment and orders?**
No. This server strictly focuses on the Marketplace Catalog and Pricing to maintain secure boundaries. To manage orders, please use the `walmart-orders-mcp` server.

**Q: Can I update prices or inventory for multiple SKUs at once?**
Yes, the agent interacts with Walmart's Bulk operations endpoint to process batch updates efficiently without rate-limit throttling.

**Q: Does this agent configure limited-time promotions for special events?**
Yes. You can dynamically set promotional pricing algorithms by specifying precise start and end dates directly impacting your item's Buy Box.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/walmart-marketplace](https://vinkius.com/mcp/walmart-marketplace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Walmart Marketplace** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `walmart-marketplace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Walmart Marketplace** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "walmart-marketplace": {
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
