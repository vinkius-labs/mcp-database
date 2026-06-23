# Export Parity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/export-parity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the net farm-gate price for grain exports by accounting for logistics and taxes.

## Description
This MCP server provides tools to determine the profitability of exporting commodities like grains. By using `get_transportation_rate`, you can find the cost per kilometer for different transport modes. The `calculate_farm_gate_parity` tool computes the final net price at the farm after subtracting freight, port fees, and export taxes from the international FOB price. Finally, use `analyze_market_opportunity` to compare this parity price against domestic market prices to decide whether to export or sell locally.


## Available Tools (3)
- **calculate_farm_gate_parity**: Calculate the net price received at the farm after logistics costs
- **analyze_market_opportunity**: Analyze if export or domestic market is more profitable
- **get_transportation_rate**: Get the transport rate per km for a specific mode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Export Parity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the transport rate for a truck?"

**🤖 AI Agent:**
> The `get_transportation_rate` tool returns the cost per km and currency for the selected mode.

---

**👤 You:**
> "Calculate parity: FOB $500, Rate 5.2, Distance 500km, Mode truck, Port Fees 100, Taxes 50."

**🤖 AI Agent:**
> Using `calculate_farm_gate_parity`, the tool will compute the net farm-gate price after all deductions.

---

**👤 You:**
> "Should I export if my parity is 2500 and domestic price is 2400?"

**🤖 AI Agent:**
> The `analyze_market_opportunity` tool will recommend 'EXPORT' because the parity price is higher.


## ❓ FAQ

**Q: How do I find the transport cost for a specific mode?**
Use the `get_transportation_rate` tool and provide the mode (truck, rail, or barge).

**Q: What inputs are needed for parity calculation?**
You need the FOB price in USD, the exchange rate, distance in km, and the transport mode for `calculate_farm_gate_parity`.

**Q: Can I compare export prices with domestic prices?**
Yes, the `analyze_market_opportunity` tool compares your calculated parity price to the domestic market price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/export-parity-calculator](https://vinkius.com/mcp/export-parity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Export Parity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `export-parity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Export Parity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "export-parity-calculator": {
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
