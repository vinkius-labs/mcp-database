# Squad Budget Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/squad-budget-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Financial planning engine for football squad budgets and compliance.

## Description
This MCP server provides a comprehensive financial planning engine for football clubs. It allows AI agents to manage squad costs by calculating committed and projected budgets, analyzing transfer amortization, and simulating performance-based bonus scenarios. Use `get_squad_financial_summary` to view overall health, `calculate_player_amortization_impact` to see individual player transfer costs, `simulate_bonus_scenarios` to test trophy wins, and `validate_squad_compliance` to check wage-to-revenue ratios.


## Available Tools (4)
- **calculate_player_amortization_impact**: Determines the specific book cost impact of a player's transfer for a given period
- **get_squad_financial_summary**: Calculates the high-level financial health of a squad for a specific timeframe
- **simulate_bonus_scenarios**: Evaluates how different performance outcomes affect the total budget
- **validate_squad_compliance**: Checks the squad against specific regulatory constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Squad Budget Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current budget status for 2024-Q1?"

**🤖 AI Agent:**
> For 2024-Q1, the committed budget is €45.0M, the projected budget is €52.5M, and you have a remaining budget of €7.5M.

---

**👤 You:**
> "How much will the transfer of player P123 impact our budget this quarter?"

**🤖 AI Agent:**
> The periodic amortization for player P123 in this period is €1.2M, with a remaining contract value of €12.0M.

---

**👤 You:**
> "What happens to our budget if we trigger the 'league_winner' bonus?"

**🤖 AI Agent:**
> Triggering the 'league_winner' bonus will increase the total projected budget by €5.0M, resulting in a total projected spend of €57.5M.


## ❓ FAQ

**Q: How do I check if my squad is within the spending limit?**
You can use the `get_squad_financial_summary` tool to see the remaining budget and any rule violations relative to your cap or revenue.

**Q: Can I simulate the cost of winning a trophy?**
Yes, use the `simulate_bonus_scenarios` tool by providing the period and the specific contingent bonus identifiers you wish to test.

**Q: How is transfer cost calculated in the budget?**
The engine uses transfer amortization. You can use `calculate_player_amortization_impact` to find the specific book cost for a player in a given period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/squad-budget-calculator](https://vinkius.com/en/ai-agent-connect/squad-budget-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Squad Budget Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `squad-budget-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Squad Budget Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "squad-budget-calculator": {
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
