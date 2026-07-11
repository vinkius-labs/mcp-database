# Baggage Allowance Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/baggage-allowance-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Compare airline baggage dimensions, weight limits, and sports equipment fees.

## Description
The Baggage Allowance Comparator connects AI agents to a comprehensive database of airline policies. Use `get_cabin_bag_specifications` to check size limits and enforcement ratings, `get_checked_baggage_allowance` for weight thresholds by class, `compare_sports_equipment_fees` for gear surcharges, `calculate_excess_weight_cost` for route-based fees, and `get_airline_policy_rating` to assess policy friendliness. It provides critical data on dimensions, weights, and costs across 50+ airlines.

### Available Tools

`compare_baggage_allowance`


## Available Tools (1)
- **compare_baggage_allowance**: Compares baggage allowances between two airlines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baggage Allowance Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the cabin bag dimensions for Lufthansa?"

**🤖 AI Agent:**
> For Lufthansa, the maximum allowable dimensions are 55 x 40 x 23 cm with a lenient enforcement rating.

---

**👤 You:**
> "How much does it cost to bring a bicycle on British Airways?"

**🤖 AI Agent:**
> The flat fee for transporting a bicycle on British Airways is 50 GBP.

---

**👤 You:**
> "What is the weight limit for Business class on Emirates?"

**🤖 AI Agent:**
> The maximum weight allowed for checked luggage in Business class on Emirates is 40 kg.


## ❓ FAQ

**Q: How can I check if my carry-on fits?**
Use the `get_cabin_bag_specifications` tool with the airline name to see maximum dimensions and whether they are strictly enforced. Tools available: `compare_baggage_allowance`.

**Q: Does this tool cover sports equipment?**
Yes, you can use `compare_sports_equipment_fees` to find the cost for items like golf clubs, bicycles, and skis.

**Q: How are excess baggage fees calculated?**
The `calculate_excess_weight_cost` tool calculates fees based on the specific route region and the amount of extra weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/baggage-allowance-comparator](https://vinkius.com/mcp/baggage-allowance-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baggage Allowance Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baggage-allowance-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baggage Allowance Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baggage-allowance-comparator": {
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
