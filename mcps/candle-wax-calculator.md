# Candle Wax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/candle-wax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate precise wax weights and batch costs for candle production.

## Description
This MCP server provides essential calculation tools for candle makers. Use `get_wax_requirements` to determine the total wax weight needed for a production batch and the amount required per individual candle. You can also use `validate_fill_safety` to ensure your fill levels are safe for different vessel types like jars or tins, `convert_volume_to_weight` for quick mass conversions, and `batch_cost_estimation` to manage production expenses.


## Available Tools (4)
- **batch_cost_estimation**: Calculates the financial cost of the wax required for a specific batch
- **convert_volume_to_weight**: Provides a quick conversion between liquid volume and wax mass
- **validate_fill_safety**: Checks if a requested fill percentage is safe for the specific container type to prevent overflow or hazardous levels
- **get_wax_requirements**: Calculates the total wax needed for a full production batch and the amount per individual candle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Candle Wax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much wax do I need for 50 candles in 200ml jars with an 80% fill?"

**🤖 AI Agent:**
> You will need 8,000ml of total volume, which results in 160g of wax per candle and a total of 8,000g of wax for the batch (assuming a density factor of 1.0).

---

**👤 You:**
> "Is a 95% fill safe for a jar container?"

**🤖 AI Agent:**
> No, for jar types, the fill should not exceed 90% to allow for fragrance oil displacement.

---

**👤 You:**
> "What is the cost for 5000g of wax if it costs $0.02 per gram?"

**🤖 AI Agent:**
> The total cost for the wax batch is $100.00.


## ❓ FAQ

**Q: How do I calculate the total wax needed for my batch?**
You can use the `get_wax_requirements` tool by providing the container volume, the desired fill percentage, and the total number of candles in your batch.

**Q: Can I check if my fill level is safe for a specific jar?**
Yes, the `validate_fill_safety` tool checks if your intended fill level is within safe bounds for vessel types like jars, tins, or pillars.

**Q: How do I estimate the cost of my wax batch?**
Use the `batch_cost_estimation` tool with the total wax weight and the cost per unit weight to get the total production cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/candle-wax-calculator](https://vinkius.com/en/ai-agent-connect/candle-wax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Candle Wax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `candle-wax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Candle Wax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "candle-wax-calculator": {
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
