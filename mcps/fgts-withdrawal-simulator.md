# FGTS Withdrawal Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fgts-withdrawal-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate FGTS balances, severance penalties, and payout liquidity based on salary and tenure.

## Description
The FGTS Withdrawal Simulator provides a precise way to predict the financial impact of employment termination in Brazil. By using tools like `calculate_accumulated_balance`, `calculate_severance_penalty`, and `evaluate_payout_liquidity`, you can estimate total monthly deposits, the 40% severance fine, and how much cash will be immediately available depending on your withdrawal mode (Standard or Annual). This bridge connects AI agents to critical Brazilian labor fund calculations.


## Available Tools (3)
- **calculate_accumulated_balance**: Determines the total amount of money deposited into the FGTS account
- **calculate_severance_penalty**: Calculates the value of the fine owed upon dismissal without just cause
- **evaluate_payout_liquidity**: Simulates immediate cash availability based on withdrawal mode


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FGTS Withdrawal Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I earn 3000 BRL and have worked for 24 months, what is my accumulated FGTS balance?"

**🤖 AI Agent:**
> Your total accumulated balance is 576.00 BRL, with a monthly deposit of 240.00 BRL.

---

**👤 You:**
> "I have 5000 BRL in my FGTS. If I am dismissed without cause, how much is the penalty?"

**🤖 AI Agent:**
> The severance penalty amount is 2000.00 BRL.

---

**👤 You:**
> "If I have 5000 BRL balance and a 2000 BRL penalty in Annual mode, how much can I withdraw immediately upon dismissal?"

**🤖 AI Agent:**
> You will have 2000.00 BRL available as immediate liquid funds, while 5000.00 BRL remains restricted.


## ❓ FAQ

**Q: How do I calculate my total FGTS balance?**
You can use the `calculate_accumulated_balance` tool by providing your monthly gross salary and the number of months you have been employed.

**Q: How is the severance penalty calculated?**
The `calculate_severance_penalty` tool calculates a 40% fine based on the total amount deposited in your account during your contract.

**Q: What is the difference between Standard and Annual withdrawal modes?**
Using `evaluate_payout_liquidity`, you can see that Standard mode allows full access to both balance and penalty upon dismissal, while Annual mode restricts the main balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fgts-withdrawal-simulator](https://vinkius.com/mcp/fgts-withdrawal-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FGTS Withdrawal Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fgts-withdrawal-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FGTS Withdrawal Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fgts-withdrawal-simulator": {
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
