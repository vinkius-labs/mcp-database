# Inventory Unit Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/inventory-unit-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Aggregate and audit inventory quantities across products and locations.

## Description
This MCP server provides specialized tools for inventory reconciliation and auditing. It allows AI agents to track stock levels, breakdown inventory by location, calculate discrepancies between ledger and physical counts, and aggregate total volumes at specific sites. Use `get_product_stock_level` to find total quantities, `get_location_inventory` for location breakdowns, `calculate_inventory_discrepancy` to identify mismatches, and `aggregate_site_total` to audit site-wide volumes.


## Available Tools (4)
- **aggregate_site_total**: Get the total inventory volume at a specific site
- **calculate_inventory_discrepancy**: Calculate the discrepancy between expected and physical inventory
- **get_location_inventory**: Get the inventory breakdown for a product
- **get_product_stock_level**: Get the total stock level for a specific product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inventory Unit Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total units of product PROD-123 do we have in the entire system?"

**🤖 AI Agent:**
> There are 550 total units of product PROD-123 stored across 3 different locations.

---

**👤 You:**
> "Is there a mismatch for product PROD-999? We expected 100 units but only counted 95."

**🤖 AI Agent:**
> Yes, there is a discrepancy of 5 units for product PROD-999.

---

**👤 You:**
> "What is the total inventory volume at Warehouse-A?"

**🤖 AI Agent:**
> Warehouse-A holds a total of 1250 units across 12 unique products.


## ❓ FAQ

**Q: How can I check the total stock for a specific item?**
You can use the `get_product_stock_level` tool by providing the unique product identifier.

**Q: How do I identify if there is a stock mismatch?**
Use the `calculate_inventory_discrepancy` tool with the expected ledger quantity and the actual physical count.

**Q: Can I see where my products are stored?**
Yes, the `get_location_inventory` tool provides a breakdown of a product's inventory across all registered locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/inventory-unit-total](https://vinkius.com/en/ai-agent-connect/inventory-unit-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inventory Unit Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inventory-unit-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inventory Unit Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inventory-unit-total": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
