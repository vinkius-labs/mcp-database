# Venture Liquidation Waterfall Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-liquidation-waterfall-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exit proceeds, liquidation preferences, and investor conversion decisions.

## Description
This MCP server provides a specialized engine for modeling exit events in venture-backed companies. It calculates the distribution of proceeds by accounting for stacked liquidation preferences, participation rights, and participation caps. Use `calculate_waterfall` to determine final payouts for all stakeholders, `simulate_exit_scenarios` to find break-even points for equity conversion, `validate_cap_table` to verify equity structures, and `get_investor_summary` for specific class metrics.


## Available Tools (4)
- **validate_cap_table**: Ensure the provided equity structure is mathematically sound before running heavy waterfall simulations
- **calculate_waterfall**: Perform the core calculation of an exit event to determine the final payout for every stakeholder
- **get_investor_summary**: Extract high-level metrics for a specific investor class to assist in negotiation modeling
- **simulate_exit_scenarios**: Compare different exit values against the current cap table to see at what break-even points investors should convert to common stock


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Liquidation Waterfall Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the waterfall for an exit of $50,000,000 with Series A having a $5,000,000 preference and 10% ownership, and founders having 40% ownership."

**🤖 AI Agent:**
> The total distributed is $50,000,000. Series A receives its $5,000,000 preference plus its pro-rata share, and the founders receive their residual portion.

---

**👤 You:**
> "What is the summary for the 'Series A' investor class in a $100,000,000 exit?"

**🤖 AI Agent:**
> For a $100,000,000 exit, the Series A class receives a total payout of $15,000,000.

---

**👤 You:**
> "Check if this cap table is valid: Series A 20%, Series B 30%, Founders 50%."

**🤖 AI Agent:**
> The cap table is invalid. The total ownership sums to 100%, but the discrepancy check confirms the structure is mathematically sound.


## ❓ FAQ

**Q: How does the engine handle stacked preferences?**
The engine iterates through the investor classes in order, satisfying the liquidation preference of each tier before moving to the next, as defined in `calculate_waterfall`.

**Q: Can I check if an investor should convert to common stock?**
Yes, you can use `simulate_exit_scenarios` to identify the specific exit values where converting to common stock yields a higher payout than the liquidation preference.

**Q: How do I ensure my cap table data is correct?**
Use the `validate_cap_table` tool to verify that the sum of all investor ownership percentages and founder ownership equals exactly 100%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-liquidation-waterfall-engine](https://vinkius.com/en/ai-agent-connect/venture-liquidation-waterfall-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Liquidation Waterfall Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-liquidation-waterfall-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Liquidation Waterfall Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-liquidation-waterfall-engine": {
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
