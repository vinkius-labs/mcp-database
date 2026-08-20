# JR Fare Zone Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/jr-fare-zone-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact Japanese JR train fares using distance-based zones and IC card discounts.

## Description
This MCP server provides deterministic tools to calculate Japanese JR train fares. It maps station pairs to specific distance zones and applies hierarchical pricing rules, including express surcharges and Suica/Pasmo IC card discounts. Use `get_station_distance` to find the distance between stations, `calculate_base_fare` for standard ticket prices, and `calculate_total_fare` to compute the final amount including premium service fees and smart card savings.


## Available Tools (3)
- **calculate_total_fare**: Compute the final amount a passenger must pay, including surcharges and IC card discounts
- **get_station_distance**: Find the exact distance in kilometers between two specific stations on a given JR line
- **calculate_base_fare**: Determine the standard ticket price based on the distance traveled


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JR Fare Zone Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is the fare from Tokyo to Shinjuku on the Yamanote Line?"

**🤖 AI Agent:**
> The fare for the trip from Tokyo to Shinjuku is 170 JPY.

---

**👤 You:**
> "What is the total fare for a 50km trip with a Shinkansen surcharge using a Suica card?"

**🤖 AI Agent:**
> The total fare for a 50km trip with the express surcharge and Suica discount is 2,450 JPY.

---

**👤 You:**
> "Calculate the base fare for a 5km journey."

**🤖 AI Agent:**
> The base fare for a 5km journey is 170 JPY.


## ❓ FAQ

**Q: How are the fares calculated?**
Fares are calculated using JR East distance brackets. The `calculate_base_fare` tool determines the base price, and `calculate_total_fare` adds any express surcharges and applies the IC card discount if requested.

**Q: Does this support Suica or Pasmo cards?**
Yes. When using `calculate_total_fare`, you can set the `useIcCard` parameter to true to apply the standard IC card discount.

**Q: Can I find the distance between two specific stations?**
Yes, you can use the `get_station_distance` tool to retrieve the exact distance in kilometers for a specific JR line.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/jr-fare-zone-calculator](https://vinkius.com/ai-agent-connect/jr-fare-zone-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JR Fare Zone Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jr-fare-zone-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JR Fare Zone Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jr-fare-zone-calculator": {
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
