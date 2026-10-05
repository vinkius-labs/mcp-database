# Product Pricing Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/product-pricing-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise product retail prices by aggregating material, labor, and overhead costs.

## Description
This MCP server provides a complete pricing engine for manufacturing and retail. It allows AI agents to calculate the total cost of goods sold (COGS) using `calculate_production_cost`, determine final customer pricing with `compute_retail_price`, and retrieve specific material unit costs via `get_material_costs`. You can also perform financial modeling with `analyze_margin_sensitivity` to see how different profit margins impact your final price. It is designed to bridge the gap between raw production data and final retail strategy.


## Available Tools (4)
- **calculate_production_cost**: Determines the base cost to manufacture a single unit
- **compute_retail_price**: Calculates the final selling price based on desired profitability
- **get_material_costs**: Retrieve the unit cost of specific raw materials used in production
- **analyze_margin_sensitivity**: Helps the user understand how changing the margin or fees affects the final price


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Pricing Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost to produce a unit if materials cost $15, labor is 2 hours at $25/hr, packaging is $2, and overhead is $5?"

**🤖 AI Agent:**
> The total base production cost is $72.00.

---

**👤 You:**
> "Calculate the final retail price for a product with a $50 production cost, a 30% target margin, 15% fulfillment fee, $10 shipping, and 8% tax."

**🤖 AI Agent:**
> The final price the customer pays is $102.60.

---

**👤 You:**
> "How much does a material with ID 'MAT-001' cost?"

**🤖 AI Agent:**
> The unit cost for MAT-001 is $4.50.


## ❓ FAQ

**Q: How do I calculate the base cost of my product?**
You can use the `calculate_production_cost` tool. You will need to provide the material costs, labor hours, hourly wage, packaging cost, and the overhead allocated per unit.

**Q: Can I see how different margins affect my final price?**
Yes, the `analyze_margin_sensitivity` tool generates scenarios showing how varying your profit margin affects the final price and profit amount.

**Q: How are taxes and fulfillment fees handled?**
The `compute_retail_price` tool accounts for both the marketplace fulfillment fee rate and the applicable sales tax or VAT rate to ensure the final price covers all costs and target margins.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/product-pricing-builder](https://vinkius.com/en/ai-agent-connect/product-pricing-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Pricing Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-pricing-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Pricing Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-pricing-builder": {
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
