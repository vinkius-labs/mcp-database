# Y Combinator Deal Economics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/y-combinator-deal-economics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate YC equity stakes, dilution, and deal scenarios.

## Description
This MCP server provides tools to model Y Combinator deal economics. Use `get_yc_equity_breakdown` to determine immediate equity stakes, `project_series_a_dilution` to forecast ownership after a Series A round, and `compare_deal_scenarios` to evaluate how different valuation caps impact final ownership. It accounts for standard YC terms including the $500k investment structure and MFN provisions.


## Available Tools (3)
- **get_yc_equity_breakdown**: Determine the immediate equity stake YC holds after the initial investment
- **project_series_a_dilution**: Calculate what YC's ownership will look like after the company completes its Series A funding round
- **compare_deal_scenarios**: Compare the outcomes of different valuation caps on YC's final ownership


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Y Combinator Deal Economics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the equity stake for a $500,000 investment with a $10,000,000 valuation cap?"

**🤖 AI Agent:**
> The total equity stake is 10% (7% from the fixed portion and 3% from the SAFE portion).

---

**👤 You:**
> "If YC owns 10% and the company raises $5M at a $20M pre-money valuation, what is the new ownership?"

**🤖 AI Agent:**
> The post-Series A ownership will be 8%.

---

**👤 You:**
> "Compare a $500k investment with caps of $5M, $10M, and $15M given a $20M next round valuation."

**🤖 AI Agent:**
> At a $5M cap, equity is 17%; at a $10M cap, equity is 12%; at a $15M cap, equity is 10.33%.


## ❓ FAQ

**Q: How does this tool handle YC's standard terms?**
The `get_yc_equity_breakdown` tool is designed to model the standard $500,000 investment, splitting it into the fixed equity portion and the SAFE portion.

**Q: Can I simulate Series A dilution?**
Yes, you can use `project_series_a_dilution` to calculate how much ownership remains after a new funding round is completed.

**Q: What is the purpose of comparing scenarios?**
The `compare_deal_scenarios` tool allows you to see how different valuation caps change the effective valuation and equity percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/y-combinator-deal-economics-calculator](https://vinkius.com/ai-agent-connect/y-combinator-deal-economics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Y Combinator Deal Economics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `y-combinator-deal-economics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Y Combinator Deal Economics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "y-combinator-deal-economics-calculator": {
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
