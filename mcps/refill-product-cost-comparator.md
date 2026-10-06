# Refill Product Cost Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refill-product-cost-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Compare the economic feasibility of single-use vs refillable packaging systems.

## Description
This MCP server provides tools to evaluate the lifecycle costs of different packaging models. It allows users to calculate unit costs for single-use products using `calculate_single_use_unit_cost` and refillable systems using `calculate_refill_unit_cost`. You can directly compare these models with `compare_refill_feasibility` or determine the exact point of economic advantage using `get_break_even_trips`.


## Available Tools (4)
- **compare_refill_feasibility**: Compares a single-use product directly against a refillable system to find the cost-per-unit difference
- **get_break_even_trips**: Calculates how many refill trips are required for the refillable system to become cheaper than the single-use option
- **calculate_single_use_unit_cost**: Determines the cost of a single-use product per unit of quantity
- **calculate_refill_unit_cost**: Determines the cost of a refillable product per unit of quantity across multiple uses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refill Product Cost Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the unit cost for a 500ml single-use bottle that costs $5.00 with a packaging factor of 1.2."

**🤖 AI Agent:**
> The unit cost for the single-use product is $0.012 per ml.

---

**👤 You:**
> "Compare a single-use product (price $5, quantity 500, packaging factor 1.2) against a refillable system (refill price $3, container price $2, quantity 500, trips 5, transport factor 1.1, packaging factor 1.0)."

**🤖 AI Agent:**
> The refillable system is cheaper, providing a savings of $0.0024 per unit and a total savings of $0.012 over 5 trips.

---

**👤 You:**
> "How many trips are needed to break even if the single-use unit price is $0.012 and the refill system has a refill price of $3, container price of $2, quantity of 500, transport factor 1.1, and packaging factor 1.0?"

**🤖 AI Agent:**
> You need at least 10 trips for the refillable system to become more economical than the single-use option.


## ❓ FAQ

**Q: How does the tool account for container deposits?**
The `calculate_refill_unit_cost` tool accepts an optional `containerDeposit` parameter, which is included in the total cost calculation for the refillable system.

**Q: What is a transport factor?**
The transport factor is a multiplier used to adjust costs based on the logistics and movement of goods, which can differ significantly between single-use and refillable models.

**Q: Can I find out when refilling becomes cheaper than buying single-use?**
Yes, you can use the `get_break_even_trips` tool to calculate the minimum number of refill cycles required for the refillable system to be more economical than the single-use option.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refill-product-cost-comparator](https://vinkius.com/en/ai-agent-connect/refill-product-cost-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refill Product Cost Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refill-product-cost-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refill Product Cost Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refill-product-cost-comparator": {
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
