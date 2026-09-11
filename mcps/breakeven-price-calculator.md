# Breakeven Price Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/breakeven-price-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Determine minimum commodity prices for oil and gas projects using NPV and full-cycle modeling.

## Description
This MCP server provides advanced financial modeling for energy projects. It calculates the minimum commodity price required to cover operating costs, initial capital investments, and target returns. By accounting for production profiles, royalty rates, and taxation, it allows for precise economic analysis. Use `calculate_operating_breakeven` to find the price needed for daily operations, `calculate_full_cycle_breakeven` for total project recovery, and `calculate_npv_breakeven` to ensure a specific target return. You can also use `compare_breakeven_scenarios` to analyze how changes in fiscal terms like tax or royalty impact your project's economics.


## Available Tools (4)
- **calculate_full_cycle_breakeven**: Calculate the price needed to cover both initial investments (CAPEX) and operating costs (OPEX)
- **calculate_npv_breakeven**: Calculate the price required to achieve a specific target return (NPV = 0) considering time value of money
- **calculate_operating_breakeven**: Calculate the minimum price needed to cover operating costs (OPEX) only
- **compare_breakeven_scenarios**: Analyze how changing the tax rate or royalty impacts the required breakeven price


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breakeven Price Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the operating breakeven price for a project with 100,000 barrels in year 1 and 50,000 in year 2, with annual costs of 10,000,000 and a 10% royalty?"

**🤖 AI Agent:**
> The minimum price required to cover operating costs is $115.42 per barrel.

---

**👤 You:**
> "Calculate the NPV breakeven price for a project with a 10% discount rate, 20% tax, and 5% royalty."

**🤖 AI Agent:**
> The price required to achieve a 10% return is $75.50 per barrel.

---

**👤 You:**
> "How much does increasing the royalty from 0.1 to 0.15 affect the breakeven price?"

**🤖 AI Agent:**
> Increasing the royalty rate from 10% to 15% increases the required breakeven price by $4.25 per barrel.


## ❓ FAQ

**Q: What is the difference between operating and full-cycle breakeven?**
Operating breakeven is the price needed to cover only ongoing expenses (OPEX), while full-cycle breakeven includes both operating costs and the initial capital investment (CAPEX).

**Q: How does the tool handle government royalties?**
The tools incorporate the royalty rate as a percentage of gross revenue, reducing the net cash flow available to cover costs and investments.

**Q: Can I compare different tax scenarios?**
Yes, you can use `compare_breakeven_scenarios` to see how varying the tax rate or royalty rate changes the required breakeven price.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/breakeven-price-calculator](https://vinkius.com/ai-agent-connect/breakeven-price-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breakeven Price Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breakeven-price-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breakeven Price Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breakeven-price-calculator": {
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
