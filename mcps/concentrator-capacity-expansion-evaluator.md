# Concentrator Capacity Expansion Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concentrator-capacity-expansion-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Evaluates capital expenditures and economic viability for concentrator capacity increases.

## Description
This MCP server provides specialized tools for mining engineers and financial analysts to evaluate concentrator capacity expansion. It allows for comparing different strategies like debottlenecking versus new line installation. Use `analyze_expansion_options` to determine physical and financial characteristics, `calculate_expansion_economics` to find net value and annualized return, `compare_expansion_strategies` to rank options by efficiency, and `validate_constraints` to ensure proposed expansions stay within physical site limits.


## Available Tools (4)
- **analyze_expansion_options**: Compares different expansion strategies to determine their physical and financial characteristics
- **calculate_expansion_economics**: Determines the financial viability of a specific expansion option
- **compare_expansion_strategies**: Ranks different expansion options based on their net value
- **validate_constraints**: Ensures a proposed expansion is physically and logically compatible with the current facility state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concentrator Capacity Expansion Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare two expansion options: a debottlenecking option with 50 units added at 100 cost, and a new line with 200 units added at 500 cost. Revenue per unit is 10 and life is 5 years."

**🤖 AI Agent:**
> The new line is the most efficient option with a net value of 500 and an efficiency ratio of 1.0, compared to the debottlenecking option which has a net value of 400.

---

**👤 You:**
> "Is it feasible to add 500 units of capacity if the current capacity is 1000 and the max facility limit is 1200?"

**🤖 AI Agent:**
> No, the expansion is infeasible because the resulting total capacity of 1500 exceeds the maximum facility limit of 1200.

---

**👤 You:**
> "Calculate the economics for an expansion with 100 incremental capacity, 50 CAPEX, 20 revenue per unit, and a 10 year life."

**🤖 AI Agent:**
> The expansion has a total CAPEX of 50, total incremental revenue of 2000, a net value of 1950, and an annualized return of 195.


## ❓ FAQ

**Q: How do I compare debottlenecking vs new line installation?**
You can use `analyze_expansion_options` to get the characteristics of both paths, then use `compare_expansion_strategies` to rank them based on net value.

**Q: Can I check if an expansion is physically possible?**
Yes, use the `validate_constraints` tool to check if a proposed expansion exceeds the maximum facility limit.

**Q: How is the economic return calculated?**
The `calculate_expansion_economics` tool calculates the net value by subtracting CAPEX from total incremental revenue, then provides the annualized return.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concentrator-capacity-expansion-evaluator](https://vinkius.com/ai-agent-connect/concentrator-capacity-expansion-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concentrator Capacity Expansion Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concentrator-capacity-expansion-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concentrator Capacity Expansion Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concentrator-capacity-expansion-evaluator": {
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
