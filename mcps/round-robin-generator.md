# Round Robin Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/round-robin-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate all possible smaller parlays from a larger set of bets.

## Description
The Round Robin Generator MCP allows AI agents to calculate every unique subset of legs for a specified group size. Using tools like `generate_all_combinations`, you can identify all possible parlays from a pool of bets, determine the uniform stake per parlay with `calculate_per_parlay_wager`, and estimate potential returns using `project_payouts`.


## Available Tools (3)
- **generate_all_combinations**: Identify every unique subset of legs for a specified group size
- **calculate_per_parlay_wager**: Determine the specific amount of money to stake on each individual combination
- **project_payouts**: Estimate the monetary return for each parlay in the set based on their odds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Round Robin Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 4 bets: 'Lakers', 'Celtics', 'Bulls', and 'Suns'. I want to play 2-leg teasers. How many combinations are there?"

**🤖 AI Agent:**
> There are 6 possible 2-leg combinations: ['Lakers', 'Celtics'], ['Lakers', 'Bulls'], ['Lakers', 'Suns'], ['Celtics', 'Bulls'], ['Celtics', 'Suns'], and ['Bulls', 'Suns'].

---

**👤 You:**
> "If I have a total wager of $100 for 6 combinations, what is my stake per parlay?"

**🤖 AI Agent:**
> Your stake per parlay will be $16.67.

---

**👤 You:**
> "Calculate the potential payout for a 2-leg parlay consisting of 'TeamA' (odds 2.0) and 'TeamB' (odds 1.5) with a $10 stake."

**🤖 AI Agent:**
> The potential payout for this parlay is $30.00.


## ❓ FAQ

**Q: What is a Round Robin in betting?**
A Round Robin is a strategy that spreads a single wager across multiple different parlays by generating every possible combination of a specific size from a larger pool of legs.

**Q: How do I calculate the stake for each parlay?**
You can use the `calculate_per_parlay_wager` tool. It divides your total budget by the number of combinations generated to ensure a uniform stake across all parlays.

**Q: Can I estimate my potential returns?**
Yes, the `project_payouts` tool estimates the monetary return for each parlay by multiplying the stake per parlay by the product of the decimal odds of all legs in that combination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/round-robin-generator](https://vinkius.com/mcp/round-robin-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Round Robin Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `round-robin-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Round Robin Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "round-robin-generator": {
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
