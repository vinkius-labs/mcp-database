# Mine Breakeven Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mine-breakeven-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate economic thresholds for mining operations.

## Description
This MCP server provides specialized computational tools for determining the economic thresholds of mining operations. It allows AI agents to evaluate the relationship between production costs, metal value, and output volume. Key capabilities include using `get_breakeven_metal_price` to find minimum market prices, `get_breakeven_grade` to determine required ore concentration, and `get_breakeven_production_rate` to find necessary production volumes. It also includes `get_economic_sensitivity` to analyze how cost and price fluctuations impact total profit.


## Available Tools (4)
- **get_breakeven_grade**: Determines the minimum concentration of metal required in the ore to remain profitable at a given metal price and production rate
- **get_breakeven_metal_price**: Determines the minimum market price required for the primary metal to cover all costs at a fixed production volume and grade
- **get_breakeven_production_rate**: Determines the necessary volume of production required to reach the breakeven point given specific costs and metal values
- **get_economic_sensitivity**: Evaluates how changes in metal price and operating costs impact the overall mine profitability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mine Breakeven Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the breakeven metal price if operating costs are 50, capital costs are 200, production rate is 10, and ore grade is 0.5?"

**🤖 AI Agent:**
> The breakeven metal price is 70.0.

---

**👤 You:**
> "Calculate the breakeven grade for a mine with 40 operating costs, 100 capital costs, 20 production rate, and a metal price of 150."

**🤖 AI Agent:**
> The minimum required ore grade is 0.933.

---

**👤 You:**
> "What is the necessary production rate to break even with 30 operating costs, 50 capital costs, 100 metal price, and 0.8 ore grade?"

**🤖 AI Agent:**
> The required breakeven production rate is 1.0.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the breakeven metal price, the minimum required ore grade, the necessary production rate, and perform economic sensitivity analysis.

**Q: Does it account for by-product credits?**
Yes, all tools allow for the inclusion of `byProductCredits` to adjust the net operating cost.

**Q: How do I connect this to my AI client?**
You can connect via Vinkius Edge using your personal Connection Token found in your Vinkius dashboard. It is compatible with Cursor, VS Code, Claude Desktop, and Windsurf.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mine-breakeven-analysis](https://vinkius.com/en/ai-agent-connect/mine-breakeven-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mine Breakeven Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mine-breakeven-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mine Breakeven Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mine-breakeven-analysis": {
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
