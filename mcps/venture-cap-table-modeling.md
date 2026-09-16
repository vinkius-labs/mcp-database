# Venture Cap Table Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-cap-table-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate equity ownership, dilution, and exit proceeds across funding rounds.

## Description
This MCP server provides a specialized simulation engine for modeling the evolution of equity ownership. It allows users to project how ownership changes through multiple funding rounds, accounting for option pool expansions and the conversion of convertible instruments like SAFEs and notes. Use `simulate_cap_table_evolution` to project future ownership states, `calculate_exit_distribution` to determine proceeds at a liquidity event, and `analyze_dilution_impact` to quantify the loss of control for specific shareholders.


## Available Tools (4)
- **analyze_dilution_impact**: Quantify the loss of control and value for specific shareholders across the funding lifecycle
- **calculate_exit_distribution**: Determine the specific dollar amount each shareholder receives during a liquidity event
- **get_round_participation_metrics**: Evaluate the terms of a specific proposed round
- **simulate_cap_table_evolution**: Project the state of the cap table through a sequence of planned funding events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Cap Table Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Simulate the cap table evolution for a startup starting with 1,000,000 shares, through a Seed round of $2M at a $10M pre-money valuation."

**🤖 AI Agent:**
> After the Seed round, the total shares will be 1,250,000, with the new investor holding 16.67% ownership.

---

**👤 You:**
> "What would be the exit proceeds for a founder holding 20% of the company if the company is acquired for $50,000,000 with no liquidation preferences?"

**🤖 AI Agent:**
> The founder would receive $10,000,000 in proceeds.

---

**👤 You:**
> "Calculate the dilution impact for a shareholder who started with 10% ownership and ended with 5% after three rounds."

**🤖 AI Agent:**
> The dilution factor for this shareholder is 0.5.


## ❓ FAQ

**Q: How does the tool handle convertible notes?**
The engine triggers conversion of convertible instruments during the first priced equity round, using either the valuation cap or the discounted price, whichever is lower.

**Q: Can I model option pool expansions?**
Yes, you can define option pool expansion parameters to simulate how new reserves dilute existing shareholders before a new investment round.

**Q: How are exit proceeds calculated?**
By using `calculate_exit_distribution`, the engine calculates proceeds by applying liquidation preferences to preferred shareholders first, then distributing remaining value pro-rata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-cap-table-modeling](https://vinkius.com/en/ai-agent-connect/venture-cap-table-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Cap Table Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-cap-table-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Cap Table Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-cap-table-modeling": {
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
