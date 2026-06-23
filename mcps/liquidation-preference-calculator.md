# Liquidation Preference Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liquidation-preference-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model complex equity distribution and liquidation preference scenarios during company exits.

## Description
This MCP server provides a specialized computational engine for modeling equity distribution during company exits. It allows AI agents to calculate exact proceeds distribution using `calculate_proceeds_distribution`, identify conversion breakpoints with `find_conversion_breakpoints`, and assess preference overhang via `assess_preference_overhang`. Perfect for analyzing cap table dynamics, participating vs non-participating structures, and liquidation multipliers.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Liquidation Preference Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If the exit price is $10,000,000 and my Series A has a 1x non-participating preference with 10% ownership, how much will they receive?"

**🤖 AI Agent:**
> The Series A investor will receive $1,000,000, as their pro-rata share of the exit price is equal to their liquidation preference amount.

---

**👤 You:**
> "Calculate the total preference overhang for a cap table with $5M in Series A (1x) and $2M in Series B (2x)."

**🤖 AI Agent:**
> The total preference obligation is $9,000,000 ($5,000,000 for Series A and $4,000,000 for Series B).

---

**👤 You:**
> "What happens to the distribution if I increase the exit price to $50M?"

**🤖 AI Agent:**
> At a $50,000,000 exit price, the higher valuation likely triggers conversion for non-participating shareholders, allowing them to participate pro-rata in the remaining proceeds.


## ❓ FAQ

**Q: What is liquidation preference?**
Liquidation preference determines the order and amount of cash distributed to shareholders during a liquidity event, ensuring preferred investors receive their specified multiplier before common shareholders. Tools available: `your_tool_name`.

**Q: How do I calculate the distribution of proceeds?**
Use the `calculate_proceeds_distribution` tool by providing the total exit price and a detailed cap table object containing investment amounts and preference terms.

**Q: Can I find when investors will convert to common stock?**
Yes, the `find_conversion_breakpoints` tool identifies the specific exit prices where non-participating investors would choose to convert their preferred shares into common shares.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liquidation-preference-calculator](https://vinkius.com/mcp/liquidation-preference-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Liquidation Preference Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `liquidation-preference-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Liquidation Preference Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "liquidation-preference-calculator": {
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
