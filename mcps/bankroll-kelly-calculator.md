# Bankroll Kelly Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bankroll-kelly-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Deterministic mathematical tool for calculating optimal football betting stakes using the Kelly Criterion.

## Description
This MCP server provides precise mathematical tools for managing betting capital using the Kelly Criterion. It allows AI agents to calculate optimal stake sizes based on bankroll, decimal odds, and estimated probability. Users can apply fractional Kelly multipliers to manage risk or set maximum stake caps. Key tools include `calculate_kelly_stake` for primary sizing, `verify_betting_parameters` to ensure mathematical viability, `get_bankroll_summary` for capital overview, and `compare_risk_profiles` to visualize the impact of different risk management strategies.


## Available Tools (4)
- **calculate_kelly_stake**: Calculates the optimal stake based on user-provided bankroll, odds, and probability
- **compare_risk_profiles**: Compares different fractional Kelly strategies to show the impact of risk reduction
- **get_bankroll_summary**: Provides a summary of the current betting capacity
- **verify_betting_parameters**: Validates that the input parameters are mathematically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bankroll Kelly Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stake for a $1000 bankroll with decimal odds of 2.0 and a 55% estimated probability."

**🤖 AI Agent:**
> The edge is 10%, the full Kelly stake is $100.00, and the applied stake is $100.00.

---

**👤 You:**
> "I have $500. What is the stake for odds of 3.0 and a 40% probability using a Half-Kelly approach?"

**🤖 AI Agent:**
> The edge is 20%, the full Kelly stake is $50.00, and the applied stake is $25.00.

---

**👤 You:**
> "Check if a bet with odds of 1.5 and a 60% probability is mathematically viable."

**🤖 AI Agent:**
> Yes, the bet is mathematically viable as the estimated probability is greater than the implied probability.


## ❓ FAQ

**Q: What is the Kelly Criterion?**
The Kelly Criterion is a mathematical formula used to determine the optimal size of a bet to maximize the long-term growth of a bankroll based on the perceived edge and the odds offered.

**Q: How do I use fractional Kelly sizing?**
You can use the `calculate_kelly_stake` tool and provide a `kellyFraction` value (e.g., 0.5 for Half-Kelly) to reduce volatility and protect your bankroll.

**Q: Can I limit my maximum bet amount?**
Yes, the `calculate_kelly_stake` tool accepts a `maxStakeCap` parameter to ensure the calculated stake does not exceed a specific limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bankroll-kelly-calculator](https://vinkius.com/en/ai-agent-connect/bankroll-kelly-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bankroll Kelly Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bankroll-kelly-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bankroll Kelly Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bankroll-kelly-calculator": {
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
