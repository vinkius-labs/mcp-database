# Flower Arrangement Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/flower-arrangement-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise costs, margins, and stem inventory for floral arrangements.

## Description
This MCP server provides a complete economic toolkit for the floral industry. It allows AI agents to calculate detailed cost breakdowns including stems, greenery, hard goods, labor, and transport. Use `calculate_arrangement_costs` to determine per-piece pricing and profit margins, `get_stem_inventory` to check stock levels, and `reconcile_stem_usage` to ensure orders can be fulfilled with current inventory.


## Available Tools (4)
- **calculate_arrangement_costs**: Calculates the full economic breakdown for a specific arrangement type and quantity
- **get_hard_goods_catalog**: Retrieves the cost of containers and foam
- **get_stem_inventory**: Retrieves the available inventory of stems and greenery
- **reconcile_stem_usage**: Compares required stems for an order against an existing inventory to check for sufficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flower Arrangement Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost for 50 rose arrangements with a target retail price of $45 each."

**🤖 AI Agent:**
> The total batch cost for 50 arrangements is $1,250.00, resulting in a per-piece cost of $25.00 and a total margin of 44.4%.

---

**👤 You:**
> "Do I have enough inventory in 'inv_123' to make 20 bouquets requiring 100 lilies?"

**🤖 AI Agent:**
> The inventory is sufficient. You have a surplus of 15 lilies.

---

**👤 You:**
> "What is the price of a standard glass vase in the hard goods catalog?"

**🤖 AI Agent:**
> The standard glass vase is priced at $4.50 per unit.


## ❓ FAQ

**Q: How does the tool handle waste in floral orders?**
The `calculate_arrangement_costs` tool includes a waste cost calculated as a percentage of the total stem and greenery cost to account for broken or wilting stems.

**Q: Can I check if I have enough flowers for a large order?**
Yes, you can use `reconcile_stem_usage` to compare the required stems for an order against your existing inventory to identify any shortfalls.

**Q: What hard goods are included in the cost calculation?**
The tool accounts for containers and structural supplies like foam, which can be looked up using `get_hard_goods_catalog`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/flower-arrangement-cost-calculator](https://vinkius.com/en/ai-agent-connect/flower-arrangement-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flower Arrangement Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flower-arrangement-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flower Arrangement Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flower-arrangement-cost-calculator": {
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
