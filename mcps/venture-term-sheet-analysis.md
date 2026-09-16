# Venture Term Sheet Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-term-sheet-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze venture capital term sheet economics, ownership dilution, and exit waterfalls.

## Description
This MCP server provides advanced modeling for venture capital financing. It allows AI agents to calculate post-investment ownership structures using `calculate_ownership_structure`, simulate cash distributions during liquidity events with `simulate_exit_waterfall`, compare the impact of different valuation offers via `evaluate_valuation_impact`, and verify compliance with investor rights using `analyze_protective_provisions`.


## Available Tools (4)
- **analyze_protective_provisions**: Determines if specific exit scenarios violate standard investor rights or protective clauses
- **evaluate_valuation_impact**: Compares the economic reality of different valuation offers
- **simulate_exit_waterfall**: Calculates the cash distribution to each stakeholder during a liquidity event
- **calculate_ownership_structure**: Determines the ownership percentages of all parties following the investment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Term Sheet Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ownership structure for a $5M pre-money valuation with a $2M investment and a 10% option pool."

**🤖 AI Agent:**
> The post-money valuation is $7,000,000. The investor ownership is 28.57%, the option pool is 10.00%, and the founder ownership is 61.43%.

---

**👤 You:**
> "If there is a $10M exit with a 1x non-participating liquidation preference for a 20% investor, how much do they get?"

**🤖 AI Agent:**
> The investor will receive $2,000,000, which is their 20% pro-rata share of the $10,000,000 exit.

---

**👤 You:**
> "Compare a $10M pre-money valuation vs an $11M pre-money valuation for a $2M investment."

**🤖 AI Agent:**
> Increasing the pre-money valuation from $10M to $11M reduces founder dilution by approximately 1.82%.


## ❓ FAQ

**Q: How does the option pool affect founder ownership?**
The option pool is typically carved out of the pre-money valuation, meaning the dilution is absorbed by existing shareholders, reducing the founders' final ownership percentage.

**Q: What is the difference between participating and non-participating liquidation preferences?**
Non-participating investors choose between their liquidation preference or their pro-rata share. Participating investors receive their preference and then share in the remaining proceeds.

**Q: Can I simulate an exit scenario?**
Yes, you can use `simulate_exit_waterfall` to calculate exactly how proceeds are distributed among stakeholders based on their specific rights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-term-sheet-analysis](https://vinkius.com/en/ai-agent-connect/venture-term-sheet-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Term Sheet Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-term-sheet-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Term Sheet Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-term-sheet-analysis": {
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
