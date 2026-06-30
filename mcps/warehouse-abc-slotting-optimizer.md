# Warehouse ABC Slotting Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/warehouse-abc-slotting-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimize warehouse SKU placement using ABC analysis to minimize travel distance.

## Description
The Warehouse ABC Slotting Optimizer connects AI agents to your warehouse logistics data. By analyzing picking frequency, it classifies SKUs into A, B, and C categories. Use `classify_sku_velocity` to identify high-velocity items, `create_slotting_plan` to assign them to the Golden Zone or other accessible areas, and `calculate_optimization_efficiency` to estimate distance reduction. This tool helps reduce picker travel time and improve ergonomic efficiency in any warehouse environment.


## Available Tools (3)
- **create_slotting_plan**: Generate a warehouse slotting plan
- **calculate_optimization_efficiency**: Calculate optimization efficiency metrics
- **classify_sku_velocity**: Classify SKUs into ABC classes based on frequency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Warehouse ABC Slotting Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify these SKUs: [{'skuId': 'SKU001', 'frequency': 500}, {'skuId': 'SKU002', 'frequency': 50}, {'skuId': 'SKU003', 'frequency': 5}]"

**🤖 AI Agent:**
> [{'skuId': 'SKU001', 'class': 'A'}, {'skuId': 'SKU002', 'class': 'B'}, {'skuId': 'SKU003', 'class': 'C'}]

---

**👤 You:**
> "Generate a slotting plan for SKU 'SKU-99' which is Class A."

**🤖 AI Agent:**
> [{'skuId': 'SKU-99', 'zoneName': 'Golden Zone', 'shelfLevel': 'Waist Level'}]

---

**👤 You:**
> "If my baseline distance is 1000m and optimized is 750m, what is the efficiency gain?"

**🤖 AI Agent:**
> The distance reduction is 25% with an estimated efficiency gain of 25%.


## ❓ FAQ

**Q: What is ABC analysis in warehouse slotting?**
ABC analysis categorizes SKUs based on their picking frequency. Class A items are high-velocity and should be placed in the 'Golden Zone' for easy access.

**Q: How can I use the `classify_sku_velocity` tool?**
Provide a JSON array of objects, each containing an `skuId` and its picking `frequency`. The tool will return the A, B, or C classification for each SKU.

**Q: What does the `create_slotting_plan` tool provide?**
It takes your existing SKU classifications and recommends specific warehouse zones, such as 'Golden Zone' for Class A or 'Remote/High' for Class C.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/warehouse-abc-slotting-optimizer](https://vinkius.com/mcp/warehouse-abc-slotting-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Warehouse ABC Slotting Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `warehouse-abc-slotting-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Warehouse ABC Slotting Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "warehouse-abc-slotting-optimizer": {
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
