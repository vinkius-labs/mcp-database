# Spa Product Inventory Forecaster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/spa-product-inventory-forecaster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Forecast spa product inventory needs and calculate reorder points.

## Description
This MCP server provides specialized inventory management tools for spa operations. It helps managers prevent stockouts by calculating safety stock and reorder points using `calculate_reorder_thresholds`. You can also generate complete replenishment plans with `calculate_replenishment_plan`, monitor inventory status via `analyze_stock_health`, and project future consumption using `predict_usage_patterns` to account for both standard usage and upcoming booking spikes.


## Available Tools (4)
- **analyze_stock_health**: Provides a high-level status report on whether a product is well-stocked, at risk, or in a stockout state
- **calculate_reorder_thresholds**: Determines the safety stock and the reorder point for a specific product
- **calculate_replenishment_plan**: Determines how much to order and when to place the order
- **predict_usage_patterns**: Projects future inventory depletion by combining standard usage and scheduled booking spikes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spa Product Inventory Forecaster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the reorder point for product ID 'oil-123' if I use 5 units a day, have 10 units needed for bookings, a 3-day lead time, and a service level of 1.5?"

**🤖 AI Agent:**
> The reorder point for 'oil-123' is 25 units, with a safety stock of 10 units.

---

**👤 You:**
> "I have 50 units of cleanser left. The reorder point is 20, I use 2 per day, and I have 10 units needed for bookings with a 4-day lead time. What should my replenishment plan be?"

**🤖 AI Agent:**
> You should order 40 units. You have 15 days remaining until you hit the reorder point.

---

**👤 You:**
> "Check the stock health for product 'mask-01'. I have 15 units, the reorder point is 20, and I have 5 units needed for bookings."

**🤖 AI Agent:**
> The stock status is At Risk with a risk level of 0.8.


## ❓ FAQ

**Q: How do I know when to order more massage oil?**
You can use `calculate_reorder_thresholds` to find your reorder point, then use `calculate_replenishment_plan` to determine exactly how much to order and when.

**Q: Can this tool account for busy weekends with many bookings?**
Yes, by using the `bookingDemand` parameter in tools like `predict_usage_patterns`, the system incorporates scheduled client activity into its forecasts.

**Q: How can I check if my current stock levels are safe?**
Use the `analyze_stock_health` tool to receive a status report (Healthy, At Risk, or Critical) based on your current stock and reorder points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/spa-product-inventory-forecaster](https://vinkius.com/en/ai-agent-connect/spa-product-inventory-forecaster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spa Product Inventory Forecaster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spa-product-inventory-forecaster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spa Product Inventory Forecaster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spa-product-inventory-forecaster": {
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
