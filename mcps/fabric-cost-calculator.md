# Fabric Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fabric-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate fabric procurement costs including waste, MOQ, and bulk discounts.

## Description
This MCP server provides specialized tools for textile procurement calculations. It allows AI agents to determine exact fabric costs by accounting for real-world manufacturing factors like cutting waste, Minimum Order Quantities (MOQ), and tiered bulk discounts. Use `calculate_basic_fabric_cost` for simple length-based pricing, `calculate_cost_with_waste` to include production loss, `calculate_cost_with_moq` to handle supplier minimums, and `apply_bulk_discount` to find the best price for large orders.


## Available Tools (4)
- **apply_bulk_discount**: Calculate cost with bulk discounts applied
- **calculate_basic_fabric_cost**: Calculate the base cost for a specific length of fabric
- **calculate_cost_with_moq**: Calculate fabric cost considering a Minimum Order Quantity (MOQ)
- **calculate_cost_with_waste**: Calculate fabric cost accounting for cutting waste


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fabric Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost for 50 meters of fabric at $5 per meter?"

**🤖 AI Agent:**
> The total cost for 50 meters of fabric at $5 per meter is $250.

---

**👤 You:**
> "I need 100 meters of fabric at $10 per meter, but I expect 15% waste. How much will it cost?"

**🤖 AI Agent:**
> Including 15% waste, you will need to purchase 115 meters, resulting in a total cost of $1,150.

---

**👤 You:**
> "The supplier has a minimum order of 20 meters. If I only need 15 meters at $8 per meter, what is my cost?"

**🤖 AI Agent:**
> Since the minimum order is 20 meters, you will be billed for 20 meters, making the total cost $160.


## ❓ FAQ

**Q: How does the waste calculation work?**
The `calculate_cost_with_waste` tool adds a specified percentage to the required length to ensure you purchase enough fabric to cover cutting and pattern placement losses.

**Q: Can I calculate costs for suppliers with minimum orders?**
Yes, use `calculate_cost_with_moq` to determine the total cost if your required length is below the supplier's Minimum Order Quantity.

**Q: Does this tool support bulk discounts?**
Yes, the `apply_bulk_discount` tool allows you to input various quantity thresholds to find the most cost-effective price per unit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fabric-cost-calculator](https://vinkius.com/en/ai-agent-connect/fabric-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fabric Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fabric-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fabric Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fabric-cost-calculator": {
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
