# Freight Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freight-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and compare shipping costs across road, rail, air, sea, and multimodal transport modes.

## Description
The Freight Cost Calculator is a specialized logistics engine that provides precise cost and time estimates for shipments. By analyzing parameters such as origin region (USA or Europe), distance, weight, volume, and cargo type, it calculates estimated USD costs and transit durations. Use `estimate_mode_cost` to get specific details for one mode, `compare_all_modes` to see a full breakdown of all available options, or `get_logistics_recommendation` to find the best strategy based on whether you prioritize speed or budget. The engine accounts for volumetric weight and regional pricing differences to ensure accurate logistics planning.


## Available Tools (3)
- **compare_all_modes**: Compare all available transport modes for a shipment
- **estimate_mode_cost**: Calculate cost and time for a specific transport mode
- **get_logistics_recommendation**: Get a logistics recommendation based on priority


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freight Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to ship 500kg of standard cargo from the USA to a destination 1000 miles away using air transport?"

**🤖 AI Agent:**
> The estimated cost for air transport is $1,250.00 with an expected transit time of 3 days.

---

**👤 You:**
> "Compare all shipping modes for 2000kg of fragile cargo in Europe, covering a distance of 500km."

**🤖 AI Agent:**
> For your shipment in Europe: Road: $450 (2 days), Rail: $380 (5 days), Air: $1,100 (1 day), Sea: $250 (12 days), Multimodal: $400 (4 days).

---

**👤 You:**
> "I need the cheapest way to move 5000kg of bulk cargo from the USA to Europe (approx. 6000km)."

**🤖 AI Agent:**
> The recommended mode for cost priority is sea transport, with an estimated cost of $2,800 and a transit time of 25 days.


## ❓ FAQ

**Q: How is the shipping cost calculated?**
The cost is determined by scaling a regional base rate against the product of weight and distance, adjusted by the cargo type multiplier. The engine also uses volumetric mass if it exceeds physical weight.

**Q: Which regions are supported?**
Currently, the calculator supports pricing models for the USA and Europe.

**Q: Can I compare different transport modes?**
Yes, you can use the `compare_all_modes` tool to see a complete breakdown of costs and transit days for road, rail, air, sea, and multimodal options.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freight-cost-calculator](https://vinkius.com/mcp/freight-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freight Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freight-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freight Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freight-cost-calculator": {
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
