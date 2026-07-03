# Kelly Criterion Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kelly-criterion-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal bet sizes using the Kelly Criterion formula.

## Description
This MCP server provides specialized tools for bankroll management and capital allocation. Use `calculate_pure_kelly` to find the mathematically optimal wager based on win probability and American odds, or `calculate_half_kelly` for a more conservative approach. You can also use `get_net_odds_ratio` to convert market odds into profit ratios and `validate_betting_parameters` to ensure your inputs are mathematically sound.


## Available Tools (4)
- **calculate_half_kelly**: Provides a safer, more conservative wagering fraction
- **calculate_pure_kelly**: Determines the maximum mathematically optimal percentage of the bankroll to wager
- **get_net_odds_ratio**: Translates American odds into the net profit-to-stake ratio (b)
- **validate_betting_parameters**: Ensures all inputs provided for any Kelly calculation are mathematically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kelly Criterion Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal bet size for a game with a 55% win probability at -110 American odds?"

**🤖 AI Agent:**
> The recommended pure Kelly wager is 4.35% of your bankroll, with a net profit ratio of 0.909.

---

**👤 You:**
> "Calculate a safe bet size for an underdog with +150 odds and a 40% chance of winning."

**🤖 AI Agent:**
> Using the Half Kelly strategy, you should wager 7.5% of your bankroll.

---

**👤 You:**
> "Convert +200 American odds to a net profit ratio."

**🤖 AI Agent:**
> The net profit ratio for +200 odds is 2.0.


## ❓ FAQ

**Q: What is the difference between Pure Kelly and Half Kelly?**
Pure Kelly calculates the maximum mathematically optimal percentage of your bankroll to wager. Half Kelly divides that result by two, providing a safer buffer against volatility and estimation errors.

**Q: How do I use American odds with this tool?**
You can input standard American format odds, such as -110 for favorites or +150 for underdogs. The `get_net_odds_ratio` tool will handle the conversion to a profit ratio automatically.

**Q: Can I verify if my win probability is valid?**
Yes, you can use the `validate_betting_parameters` tool to check if your win probability (between 0 and 1) and American odds are mathematically valid for calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kelly-criterion-sizing](https://vinkius.com/mcp/kelly-criterion-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kelly Criterion Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kelly-criterion-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kelly Criterion Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kelly-criterion-sizing": {
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
