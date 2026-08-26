# Token Vesting Claim Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/token-vesting-claim-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Optimize token claims by balancing price, gas, and tax.

## Description
This MCP server provides a deterministic optimization engine to identify the mathematically optimal time to claim vested tokens. It analyzes vesting schedules, market volatility, and gas costs to generate actionable signals. Use `analyze_vesting_status` to calculate current eligibility, `evaluate_claim_signal` to check if market conditions justify a claim, and `optimize_claim_timing` to decide between immediate execution or waiting for a market bounce based on 20-day moving averages.


## Available Tools (3)
- **analyze_vesting_status**: Calculates the current state of a specific vesting contract
- **optimize_claim_timing**: Decides the specific execution strategy based on market trends
- **evaluate_claim_signal**: Determines if the conditions are met to trigger a "Claim" action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Token Vesting Claim Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my current vesting status for a schedule starting 2023-01-01 and ending 2024-01-01 with 1000 tokens total."

**🤖 AI Agent:**
> As of today, you have 500 tokens vested and 500 tokens remaining unclaimed.

---

**👤 You:**
> "Should I claim my tokens now given the current price is $2.00 and the 20-day MA is $1.80?"

**🤖 AI Agent:**
> The price is in an uptrend. Recommendation: Claim Immediately.

---

**👤 You:**
> "Is it a good time to claim if the token price just dropped 25% in the last week?"

**🤖 AI Agent:**
> No, the volatility filter has suppressed the claim signal due to the significant price drop.


## ❓ FAQ

**Q: How does the tool decide when to claim?**
The engine triggers a claim signal when the unclaimed value exceeds $1,000 and either the token price has gained 20% since vesting started or gas costs are below 0.1% of the unclaimed value.

**Q: What is the difference between the claim tools?**
You can use `analyze_vesting_status` to see how many tokens are ready, `evaluate_claim_signal` to see if it is profitable to claim now, and `optimize_claim_timing` to determine if you should wait for a market uptrend.

**Q: Does this account for gas prices?**
Yes, the engine includes a gas ceiling (50 gwei) and evaluates gas efficiency relative to the token value to ensure profitability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/token-vesting-claim-strategy](https://vinkius.com/ai-agent-connect/token-vesting-claim-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Token Vesting Claim Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `token-vesting-claim-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Token Vesting Claim Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "token-vesting-claim-strategy": {
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
