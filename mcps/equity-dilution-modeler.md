# Equity Dilution Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/equity-dilution-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model ownership changes and dilution across multiple venture capital funding rounds.

## Description
This MCP server provides precision tools for modeling the impact of venture capital investment rounds on existing ownership structures. Use `get_round_impact` to calculate immediate dilution from a single round, or `simulate_waterfall` to project ownership changes across a sequence of multiple funding stages. It also includes specialized tools like `calculate_pro_rata_participation` to determine required investments for maintaining stakes and `check_anti_dilution_trigger` to evaluate the impact of down rounds.


## Available Tools (4)
- **calculate_pro_rata_participation**: Determines how much capital an existing investor must contribute to maintain their ownership stake in a new round
- **check_anti_dilution_trigger**: Evaluates if a specific round qualifies as a "down round" and calculates the impact on protected investors
- **get_round_impact**: Calculates the immediate dilution effects of a single specific investment round
- **simulate_waterfall**: Projects the ownership changes across a sequence of multiple funding rounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Equity Dilution Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the impact of a $5M seed round on a founder with 100% equity if the pre-money valuation is $15M and the option pool is 10%?"

**🤖 AI Agent:**
> After the $5M seed round with a $15M pre-money valuation and a 10% option pool, the post-money valuation is $20M. The founder's equity will be 75%.

---

**👤 You:**
> "How much should an investor with 10% ownership invest in a new $10M round if the pre-money valuation is $40M?"

**🤖 AI Agent:**
> To maintain a 10% ownership stake in a $50M post-money company, the investor must contribute $5,000,000.

---

**👤 You:**
> "If the previous round price per share was $10.00 and the current round is $8.00, is a down round triggered?"

**🤖 AI Agent:**
> Yes, a down round is triggered because the current price per share is lower than the previous round price.


## ❓ FAQ

**Q: How do I model multiple funding rounds at once?**
You can use the `simulate_waterfall` tool, which accepts a starting cap table and a list of round parameters to project the entire sequence.

**Q: Can this tool help me calculate pro-rata rights?**
Yes, the `calculate_pro_rata_participation` tool determines exactly how much capital an investor must contribute to maintain their current ownership percentage.

**Q: Does it account for down rounds?**
Yes, you can use `check_anti_dilution_trigger` to evaluate if a round qualifies as a down round and calculate the resulting adjustment factors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/equity-dilution-modeler](https://vinkius.com/en/ai-agent-connect/equity-dilution-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Equity Dilution Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `equity-dilution-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Equity Dilution Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "equity-dilution-modeler": {
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
